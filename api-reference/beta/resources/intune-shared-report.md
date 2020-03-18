---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d321b5a2dadc4a459194a24224805f7443592532
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768011"
---
# <a name="report-resource-type"></a><span data-ttu-id="8944c-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="8944c-103">report resource type</span></span>

> <span data-ttu-id="8944c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8944c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8944c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8944c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8944c-106">Возвращает содержимое, подходящее для контекста, в том числе:</span><span class="sxs-lookup"><span data-stu-id="8944c-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="8944c-107">Отчеты об истории профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="8944c-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="8944c-108">Отчеты о сбоях регистрации.</span><span class="sxs-lookup"><span data-stu-id="8944c-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="8944c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8944c-109">Properties</span></span>
|<span data-ttu-id="8944c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8944c-110">Property</span></span>|<span data-ttu-id="8944c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8944c-111">Type</span></span>|<span data-ttu-id="8944c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8944c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8944c-113">содержимое</span><span class="sxs-lookup"><span data-stu-id="8944c-113">content</span></span>|<span data-ttu-id="8944c-114">Поток</span><span class="sxs-lookup"><span data-stu-id="8944c-114">Stream</span></span>|<span data-ttu-id="8944c-115">Содержимое отчета; сведения зависят от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="8944c-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8944c-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8944c-116">Relationships</span></span>
<span data-ttu-id="8944c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8944c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8944c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8944c-118">JSON Representation</span></span>
<span data-ttu-id="8944c-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8944c-119">Here is a JSON representation of the resource.</span></span>
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



