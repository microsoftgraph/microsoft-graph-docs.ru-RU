---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22bb8cd564c4ad27f3299d193f5cea6ad3cbdf75
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523585"
---
# <a name="report-resource-type"></a><span data-ttu-id="ae84e-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="ae84e-103">report resource type</span></span>

<span data-ttu-id="ae84e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ae84e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae84e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae84e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae84e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae84e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae84e-107">Возвращает содержимое, подходящее для контекста, в том числе:</span><span class="sxs-lookup"><span data-stu-id="ae84e-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="ae84e-108">Отчеты об истории профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="ae84e-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="ae84e-109">Отчеты о сбоях регистрации.</span><span class="sxs-lookup"><span data-stu-id="ae84e-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="ae84e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae84e-110">Properties</span></span>
|<span data-ttu-id="ae84e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae84e-111">Property</span></span>|<span data-ttu-id="ae84e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ae84e-112">Type</span></span>|<span data-ttu-id="ae84e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ae84e-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae84e-114">содержимое</span><span class="sxs-lookup"><span data-stu-id="ae84e-114">content</span></span>|<span data-ttu-id="ae84e-115">Поток</span><span class="sxs-lookup"><span data-stu-id="ae84e-115">Stream</span></span>|<span data-ttu-id="ae84e-116">Содержимое отчета; сведения зависят от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="ae84e-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae84e-117">Связи</span><span class="sxs-lookup"><span data-stu-id="ae84e-117">Relationships</span></span>
<span data-ttu-id="ae84e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ae84e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae84e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae84e-119">JSON Representation</span></span>
<span data-ttu-id="ae84e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae84e-120">Here is a JSON representation of the resource.</span></span>
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



