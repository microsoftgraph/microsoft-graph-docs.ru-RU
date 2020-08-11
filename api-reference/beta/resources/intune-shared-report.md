---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f017ce3ec744bb86ee3ea6e9820a0e29f8505514
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630223"
---
# <a name="report-resource-type"></a><span data-ttu-id="bb5b2-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="bb5b2-103">report resource type</span></span>

<span data-ttu-id="bb5b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb5b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb5b2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb5b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb5b2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb5b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb5b2-107">Возвращает содержимое, подходящее для контекста, в том числе:</span><span class="sxs-lookup"><span data-stu-id="bb5b2-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="bb5b2-108">Отчеты об истории профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="bb5b2-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="bb5b2-109">Отчеты о сбоях регистрации.</span><span class="sxs-lookup"><span data-stu-id="bb5b2-109">Enrollment failure reports.</span></span>
- <span data-ttu-id="bb5b2-110">Отчеты об использовании Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bb5b2-110">Microsoft 365 usage reports</span></span>

## <a name="properties"></a><span data-ttu-id="bb5b2-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb5b2-111">Properties</span></span>
|<span data-ttu-id="bb5b2-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb5b2-112">Property</span></span>|<span data-ttu-id="bb5b2-113">Тип</span><span class="sxs-lookup"><span data-stu-id="bb5b2-113">Type</span></span>|<span data-ttu-id="bb5b2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="bb5b2-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb5b2-115">содержимое</span><span class="sxs-lookup"><span data-stu-id="bb5b2-115">content</span></span>|<span data-ttu-id="bb5b2-116">Поток</span><span class="sxs-lookup"><span data-stu-id="bb5b2-116">Stream</span></span>|<span data-ttu-id="bb5b2-117">Содержимое отчета; сведения зависят от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="bb5b2-117">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb5b2-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="bb5b2-118">Relationships</span></span>
<span data-ttu-id="bb5b2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bb5b2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb5b2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb5b2-120">JSON Representation</span></span>
<span data-ttu-id="bb5b2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb5b2-121">Here is a JSON representation of the resource.</span></span>
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



