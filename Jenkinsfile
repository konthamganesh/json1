def amap = ['something': 'my datas',
                    'size': 3,
                    'isEmpty': false]

        String json = writeJSON returnText: true, json: amap
        def read = readJSON text: yml

        assert read.something == 'my datas'
        assert read.size == 3
        assert read.isEmpty == false
