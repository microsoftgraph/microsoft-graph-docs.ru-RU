---
title: Отображение изображения диаграммы в Excel
description: При извлечении изображения диаграммы API Excel в Microsoft Graph возвращает изображение в виде строки base-64, которую можно отобразить внутри htmL-тега изображения.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ac1713d017ee982c4df5fc89ff4a28dc4437a4cf
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440855"
---
# <a name="display-a-chart-image-in-excel"></a>Отображение изображения диаграммы в Excel

При выполнении [операции GET](/graph/api/chart-image) для получения изображения диаграммы API Excel в Microsoft Graph возвращает изображение в виде строки base-64. Строку base-64 можно отобразить в теге htmL-образа:

```html
 <img src="data:image/png;base64,{base-64 chart image string}/>
```

В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.

Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки. А вот как выглядит то же самое изображение диаграммы, если получить его с этими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.

## <a name="see-also"></a>См. также

* [Управление сеансами в Excel с помощью Microsoft Graph](excel-manage-sessions.md)
* [Запись в книгу Excel с помощью Microsoft Graph](excel-write-to-workbook.md)
* [Использование функций книг в Excel с помощью Microsoft Graph](excel-use-functions.md)
* [Обновление формата диапазона в Excel с помощью Microsoft Graph](excel-update-range-format.md)
* [Использование REST API для Excel](/graph/api/resources/excel)
