# A simple fork of conventional-changelog/conventional-changelog-angular

I added **design**, **animation** and **text** as nye commit types: [see changes here](https://github.com/ddennis/conventional-changelog-ddennis/commit/fa2796a1f4b0e237262b106566d11c959ba8274e)  

### Usage
    npm i https://github.com/ddennis/conventional-changelog-ddennis --save-dev
    

    
With gulp:

    gulp.task('changelog', function () {
        return gulp.src('CHANGELOG.md', {
            buffer: false
        })
            .pipe(conventionalChangelog(
                  {
                        preset:'ddennis',
                        releaseCount:0
                  }
             ))
        .pipe(gulp.dest('./'));
    });
