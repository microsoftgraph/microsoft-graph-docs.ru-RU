---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec2120660ac47fa44e700dadc34712cf3a4351e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084144"
---
# <a name="report-resource-type"></a><span data-ttu-id="b5049-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="b5049-103">report resource type</span></span>

<span data-ttu-id="b5049-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5049-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5049-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5049-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5049-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5049-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5049-107">Возвращает содержимое, подходящее для контекста, в том числе:</span><span class="sxs-lookup"><span data-stu-id="b5049-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="b5049-108">Отчеты об истории профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="b5049-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="b5049-109">Отчеты о сбоях регистрации.</span><span class="sxs-lookup"><span data-stu-id="b5049-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="b5049-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5049-110">Properties</span></span>
|<span data-ttu-id="b5049-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5049-111">Property</span></span>|<span data-ttu-id="b5049-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b5049-112">Type</span></span>|<span data-ttu-id="b5049-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b5049-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5049-114">содержимое</span><span class="sxs-lookup"><span data-stu-id="b5049-114">content</span></span>|<span data-ttu-id="b5049-115">Поток</span><span class="sxs-lookup"><span data-stu-id="b5049-115">Stream</span></span>|<span data-ttu-id="b5049-116">Содержимое отчета; сведения зависят от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="b5049-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5049-117">Связи</span><span class="sxs-lookup"><span data-stu-id="b5049-117">Relationships</span></span>
<span data-ttu-id="b5049-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b5049-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5049-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5049-119">JSON Representation</span></span>
<span data-ttu-id="b5049-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5049-120">Here is a JSON representation of the resource.</span></span>
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






