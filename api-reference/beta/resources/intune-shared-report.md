---
title: Тип ресурса report
description: 'Возвращает содержимое контексту, включая:'
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: dbad8a8808d40c2ae1f7769773b6b29ef65d680f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970649"
---
# <a name="report-resource-type"></a><span data-ttu-id="b6562-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="b6562-103">report resource type</span></span>

> <span data-ttu-id="b6562-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6562-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6562-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6562-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6562-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6562-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6562-107">Возвращает содержимое контексту, включая:</span><span class="sxs-lookup"><span data-stu-id="b6562-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="b6562-108">Отчеты журнала профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b6562-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="b6562-109">Отчеты заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="b6562-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="b6562-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6562-110">Properties</span></span>
|<span data-ttu-id="b6562-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6562-111">Property</span></span>|<span data-ttu-id="b6562-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b6562-112">Type</span></span>|<span data-ttu-id="b6562-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b6562-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6562-114">content</span><span class="sxs-lookup"><span data-stu-id="b6562-114">content</span></span>|<span data-ttu-id="b6562-115">Stream</span><span class="sxs-lookup"><span data-stu-id="b6562-115">Stream</span></span>|<span data-ttu-id="b6562-116">Отчет о содержимого; сведения в зависимости от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="b6562-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6562-117">Связи</span><span class="sxs-lookup"><span data-stu-id="b6562-117">Relationships</span></span>
<span data-ttu-id="b6562-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b6562-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6562-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6562-119">JSON Representation</span></span>
<span data-ttu-id="b6562-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6562-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



