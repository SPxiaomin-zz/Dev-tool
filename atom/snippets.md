# 代码片段

## 自带功能

- `shift + alt + s`: 查看所有的代码片段；

- `tab` 键：

    当输入 `afn` 等后，出现有多个输入点的地方，在一个地方输入完毕了之后，可以使用 `tab` 键跳到下一个位置；

## 自定义代码片段

- example:

        '.source.js':
            'ES6 module import':
                'prefix': 'mi'
                'body': 'import ${1:NAME} from \'$2\';'
                'React component':
                    'prefix': 'rec'
                    'body': """
                        class ${1:NAME} extends React.Component {
                            constructor(props) {
                                super(props);
                            }

                            render() {
                                return (
                                    $2
                                );
                            }
                        }
                    """
                'React component with export':
                    'prefix': 'recx'
                    'body': """
                        class ${1:NAME} extends React.Component {
                            constructor(props) {
                                super(props);
                            }

                            render() {
                                return (
                                    $2
                                );
                            }
                        }

                        export { ${1:NAME} as default };
                    """
