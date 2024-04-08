## SwapStation Interface

### Install Procedure
#### Use Node 16 as required
``` error detective-postcss@5.1.1: The engine "node" is incompatible with this module. Expected version "12.x || 14.x || 16.x". Got "20.12.0" ```

#### Install Node 16
``` nvm use 16 ``` # nvm install 16 and then nvm use 16

If you don thave nvm use the following --> https://heynode.com/tutorial/install-nodejs-locally-nvm

#### Yarn Install
``` yarn install ``` or ``` npm install ```

#### NPM Build
``` yarn build ``` or ``` npm run build ```

#### NPM Start
``` yarn start ``` or ``` npm run start ```

#### Troubleshooting Build Process
``` FATAL ERROR: Ineffective mark-compacts near heap limit Allocation failed - JavaScript heap out of memory ```

#### Set value of max-space-size (in MB)
``` export NODE_OPTIONS="--max-old-space-size=8192" ```

#### See the current value of max-old-space-size (in MB)
``` node -e 'console.log(v8.getHeapStatistics().heap_size_limit/(1024*1024))' ```

#### Browserslist: caniuse-lite is outdated
```  npx update-browserslist-db@latest ```