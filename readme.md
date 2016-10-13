#a simple fork of conventional-changelog/conventional-changelog-angular

Added Design and animation as my own types: [see changes here](https://github.com/ddennis/conventional-changelog-ddennis/commit/3a9dacf6474cf3315874774f85260c4052386bfd)  

#Usage
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
