---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: f94be1bcc5dfde092c6360bbdddd96d604d30a55
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939674"
---
# <a name="report-resource-type"></a><span data-ttu-id="09322-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="09322-103">report resource type</span></span>

> <span data-ttu-id="09322-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09322-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09322-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09322-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09322-106">Возвращает содержимое, подходящее для контекста, в том числе:</span><span class="sxs-lookup"><span data-stu-id="09322-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="09322-107">Отчеты об истории профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="09322-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="09322-108">Отчеты о сбоях регистрации.</span><span class="sxs-lookup"><span data-stu-id="09322-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="09322-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="09322-109">Properties</span></span>
|<span data-ttu-id="09322-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="09322-110">Property</span></span>|<span data-ttu-id="09322-111">Тип</span><span class="sxs-lookup"><span data-stu-id="09322-111">Type</span></span>|<span data-ttu-id="09322-112">Описание</span><span class="sxs-lookup"><span data-stu-id="09322-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09322-113">содержимое</span><span class="sxs-lookup"><span data-stu-id="09322-113">content</span></span>|<span data-ttu-id="09322-114">Поток</span><span class="sxs-lookup"><span data-stu-id="09322-114">Stream</span></span>|<span data-ttu-id="09322-115">Содержимое отчета; сведения зависят от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="09322-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09322-116">Связи</span><span class="sxs-lookup"><span data-stu-id="09322-116">Relationships</span></span>
<span data-ttu-id="09322-117">Нет</span><span class="sxs-lookup"><span data-stu-id="09322-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09322-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09322-118">JSON Representation</span></span>
<span data-ttu-id="09322-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09322-119">Here is a JSON representation of the resource.</span></span>
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



