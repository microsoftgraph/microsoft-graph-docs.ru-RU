---
title: Тип ресурса report
description: 'Возвращает содержимое контексту, включая:'
localization_priority: Normal
ms.openlocfilehash: b44d03c12b788b10ca332c868083bc28decc4947
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875728"
---
# <a name="report-resource-type"></a><span data-ttu-id="f3433-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="f3433-103">report resource type</span></span>

> <span data-ttu-id="f3433-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3433-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3433-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3433-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3433-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f3433-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3433-107">Возвращает содержимое контексту, включая:</span><span class="sxs-lookup"><span data-stu-id="f3433-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="f3433-108">Отчеты журнала профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3433-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="f3433-109">Отчеты заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="f3433-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="f3433-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3433-110">Properties</span></span>
|<span data-ttu-id="f3433-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3433-111">Property</span></span>|<span data-ttu-id="f3433-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f3433-112">Type</span></span>|<span data-ttu-id="f3433-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f3433-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3433-114">content</span><span class="sxs-lookup"><span data-stu-id="f3433-114">content</span></span>|<span data-ttu-id="f3433-115">Stream</span><span class="sxs-lookup"><span data-stu-id="f3433-115">Stream</span></span>|<span data-ttu-id="f3433-116">Отчет о содержимого; сведения в зависимости от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="f3433-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3433-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f3433-117">Relationships</span></span>
<span data-ttu-id="f3433-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f3433-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3433-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3433-119">JSON Representation</span></span>
<span data-ttu-id="f3433-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3433-120">Here is a JSON representation of the resource.</span></span>
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



