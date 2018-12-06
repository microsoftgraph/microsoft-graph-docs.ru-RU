---
title: Показ изображения диаграммы в Excel с помощью Microsoft Graph
description: Когда вы выполняете операцию GET, чтобы получить изображение диаграммы, API Excel возвращает изображение в виде строки в кодировке Base 64.
ms.openlocfilehash: ae721547fca9a6fe835843544bf550c5fe222426
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092727"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a><span data-ttu-id="ca10f-103">Показ изображения диаграммы в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca10f-103">Display a chart image in Excel with Microsoft Graph</span></span>

<span data-ttu-id="ca10f-104">Когда вы выполняете [операцию GET, чтобы получить изображение диаграммы](/api-reference/v1.0/api/chart-image.md), API Excel возвращает изображение в виде строки в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="ca10f-104">When you perform a [GET operation to retrieve a chart image](/api-reference/v1.0/api/chart-image.md), the Excel API returns the image as a base-64 string.</span></span>

<span data-ttu-id="ca10f-105">Вы можете отображать строку в кодировке Base 64 в HTML-теге изображения: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="ca10f-105">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="ca10f-106">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="ca10f-106">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="ca10f-107">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca10f-107">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="ca10f-109">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="ca10f-109">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="ca10f-110">А вот как выглядит то же самое изображение диаграммы, если получить его с этими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="ca10f-110">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

## <a name="see-also"></a><span data-ttu-id="ca10f-111">См. также</span><span class="sxs-lookup"><span data-stu-id="ca10f-111">See also</span></span>

* [<span data-ttu-id="ca10f-112">Управление сеансами в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca10f-112">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="ca10f-113">Запись в книгу Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca10f-113">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="ca10f-114">Использование функций книг в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca10f-114">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="ca10f-115">Обновление формата диапазона в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca10f-115">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="ca10f-116">Использование REST API для Excel</span><span class="sxs-lookup"><span data-stu-id="ca10f-116">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
