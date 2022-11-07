# Nextjs Template

> Template for building nextjs apps

## Contains

- Linting (eslint)
- Formatting (prettier)
- Tailwind
- Precommit Hooks (lefthook; automatically format files before commit)
- Database ORM (prisma)

## Usage
- Clone repository 
- Install packages `pnpm install` <br> (see below for info about pnpm)
- Copy `example.env` to `.env` and fill in required values
- Run `pnpm db:update` to sync database
- Reload IDE  <br> This allows eslint and @prisma/client to work properly with auto completion. **Do this every time you generate a new prisma client**

## Package Management (pnpm)
### **Why pnpm?**
PNPM is  similar to yarn syntactically in many ways except it is more disk space efficient than npm or yarn. This is due to the usage of symlinks so that you will never have to install the same package twice. Ex If you install react in project a and b and the react version is the same, why download it twice. Instead PNPM downloads the version of react one time and then creates symlinks to that installation in both projects.

Install pnpm by running `npm i -g pnpm` <br> Read more [here](https://pnpm.io/installation)


## License
[MIT License](https://opensource.org/licenses/MIT)