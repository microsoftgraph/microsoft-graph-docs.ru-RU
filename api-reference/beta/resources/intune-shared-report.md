---
title: Тип ресурса report
description: 'Возвращает содержимое контексту, включая:'
ms.openlocfilehash: b05e5db2b948455f14746cf23a07b3fd788ccad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080220"
---
# <a name="report-resource-type"></a><span data-ttu-id="a036d-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="a036d-103">report resource type</span></span>

> <span data-ttu-id="a036d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a036d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a036d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a036d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a036d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a036d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a036d-107">Возвращает содержимое контексту, включая:</span><span class="sxs-lookup"><span data-stu-id="a036d-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="a036d-108">Отчеты журнала профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a036d-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="a036d-109">Отчеты заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="a036d-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="a036d-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="a036d-110">Properties</span></span>
|<span data-ttu-id="a036d-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="a036d-111">Property</span></span>|<span data-ttu-id="a036d-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a036d-112">Type</span></span>|<span data-ttu-id="a036d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a036d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a036d-114">content</span><span class="sxs-lookup"><span data-stu-id="a036d-114">content</span></span>|<span data-ttu-id="a036d-115">Stream</span><span class="sxs-lookup"><span data-stu-id="a036d-115">Stream</span></span>|<span data-ttu-id="a036d-116">Отчет о содержимого; сведения в зависимости от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="a036d-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a036d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="a036d-117">Relationships</span></span>
<span data-ttu-id="a036d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a036d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a036d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a036d-119">JSON Representation</span></span>
<span data-ttu-id="a036d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a036d-120">Here is a JSON representation of the resource.</span></span>
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



