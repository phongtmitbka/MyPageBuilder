<template>
  <Section :classAttributes="classAttributes" :style="cssAttributes" :children="children" />
</template>

<script>
export default {
    data() {
        return {
            classAttributes: [
                'wrapper'
            ],
            cssAttributes: {
                background: 'white',
                height: '800px'
            },
            children: [
                {
                    type: 'section',
                    classAttributes: [
                        'container-fluid'
                    ],
                    cssAttributes: {
                        background: 'white'
                    },
                    children: [
                        {
                            type: 'section',
                            classAttributes: [
                                'container'
                            ],
                            cssAttributes: {
                                background: 'white',
                                height: '80px',
                            },
                            children: [
                                {
                                    type: 'image',
                                    classAttributes: [
                                    ],
                                    cssAttributes: {
                                        width: '64px',
                                        height: '64px',
                                    },
                                    src: 'https://mykiot-bucket.s3-ap-southeast-1.amazonaws.com/2020/04/1585793147tải xuống.png',
                                    alt: 'This is a Image',
                                    href: 'https://rautim.vn/',
                                    target: '_blank'
                                },
                                {
                                    type: 'input',
                                    classAttributes: ['col-6'],
                                    cssAttributes: {},
                                    placeHolder: 'Nhập từ khóa cần tìm',
                                    value: '',
                                }
                            ]
                        },
                        {
                            type: 'section',
                            classAttributes: [
                                'row'
                            ],
                            cssAttributes: {
                            },
                            children: [
                                {
                                    type: 'section',
                                    classAttributes: [
                                        'col-6'
                                    ],
                                    cssAttributes: {
                                    },
                                    children: [
                                        {
                                            type: 'text',
                                            classAttributes: [
                                                'text-center'
                                            ],
                                            cssAttributes: {
                                            },
                                            content: 'This is a text'
                                        },
                                        {
                                            type: 'heading',
                                            classAttributes: [
                                                'text-center'
                                            ],
                                            cssAttributes: {
                                                background: 'green'
                                            },
                                            content: 'This is a heading',
                                            headingSize: 'h1'
                                        },
                                        {
                                            type: 'heading',
                                            classAttributes: [
                                                'text-center'
                                            ],
                                            cssAttributes: {
                                                background: 'green'
                                            },
                                            content: 'This is a heading',
                                            headingSize: 'h2'
                                        },
                                        {
                                            type: 'button',
                                            classAttributes: ['btn', 'btn-primary'],
                                            cssAttributes: {},
                                            content: 'Button Primary'
                                        },
                                        {
                                            type: 'image',
                                            classAttributes: [],
                                            cssAttributes: {
                                                width: '100px',
                                                height: '100px',
                                            },
                                            src: 'https://cdn-images.kiotviet.vn/rautim/9cc872f831d7461ba604cc16feec6e70.jpg',
                                            alt: 'This is a Image',
                                        }
                                    ]
                                },
                                {
                                    type: 'section',
                                    classAttributes: [
                                        'col-6'
                                    ],
                                    cssAttributes: {
                                    },
                                    children: [

                                    ]
                                }
                            ]
                        }
                    ]
                },
                {
                    type: 'section',
                    classAttributes: [
                        'container'
                    ],
                    cssAttributes: {
                    },
                    children: [
                        {
                            type: 'section',
                            classAttributes: [
                                'row'
                            ],
                            cssAttributes: {
                            },
                            children: [
                                {
                                    type: 'section',
                                    classAttributes: [
                                        'col-6'
                                    ],
                                    cssAttributes: {
                                    },
                                    children: [
                                        {
                                            type: 'text',
                                            classAttributes: [
                                                'text-center'
                                            ],
                                            cssAttributes: {
                                            },
                                            content: 'This is a text'
                                        },
                                        {
                                            type: 'heading',
                                            classAttributes: [
                                                'text-center'
                                            ],
                                            cssAttributes: {
                                            },
                                            content: 'This is a heading',
                                            headingSize: 'h1'
                                        },
                                        {
                                            type: 'heading',
                                            classAttributes: [
                                                'text-center'
                                            ],
                                            cssAttributes: {
                                            },
                                            content: 'This is a heading',
                                            headingSize: 'h2'
                                        },
                                        {
                                            type: 'button',
                                            classAttributes: ['btn', 'btn-primary'],
                                            cssAttributes: {},
                                            content: 'Button'
                                        },
                                        {
                                            type: 'image',
                                            classAttributes: [],
                                            cssAttributes: {
                                                width: '100px',
                                                height: '100px',
                                            },
                                            src: 'https://cdn-images.kiotviet.vn/rautim/e836d8372a7e459493c06ba0db574656.jpeg',
                                            alt: 'This is a Image',
                                        }
                                    ]
                                },
                                {
                                    type: 'section',
                                    classAttributes: [
                                        'col-6'
                                    ],
                                    cssAttributes: {
                                    },
                                    children: [

                                    ]
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    }
}
</script>

<style>
</style>
