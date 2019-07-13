---
title: Показ изображения диаграммы в Excel с помощью Microsoft Graph
description: Когда вы выполняете операцию GET, чтобы получить изображение диаграммы, API Excel возвращает изображение в виде строки в кодировке Base 64.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 330c7d3a531a5735e824dda61928c3af2f05e5e3
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645217"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a>Показ изображения диаграммы в Excel с помощью Microsoft Graph

Когда вы выполняете [операцию GET, чтобы получить изображение диаграммы](/graph/api/chart-image?view=graph-rest-1.0), API Excel возвращает изображение в виде строки в кодировке Base 64.

Вы можете отображать строку в кодировке Base 64 в HTML-теге изображения: `<img src="data:image/png;base64,{base-64 chart image string}/>`.

В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`. Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки. А вот как выглядит то же самое изображение диаграммы, если получить его с этими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.

## <a name="see-also"></a>См. также

* [Управление сеансами в Excel с помощью Microsoft Graph](excel-manage-sessions.md)
* [Запись в книгу Excel с помощью Microsoft Graph](excel-write-to-workbook.md)
* [Использование функций книг в Excel с помощью Microsoft Graph](excel-use-functions.md)
* [Обновление формата диапазона в Excel с помощью Microsoft Graph](excel-update-range-format.md)
* [Использование REST API для Excel](/graph/api/resources/excel?view=graph-rest-1.0)
