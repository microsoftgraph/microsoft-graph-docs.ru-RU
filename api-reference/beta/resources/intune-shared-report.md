---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7db50d4cd4c2ced4937a594fde28eac2f4d63d0c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300537"
---
# <a name="report-resource-type"></a><span data-ttu-id="603e5-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="603e5-103">report resource type</span></span>

<span data-ttu-id="603e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="603e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="603e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="603e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="603e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="603e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="603e5-107">Возвращает содержимое, подходящее для контекста, в том числе:</span><span class="sxs-lookup"><span data-stu-id="603e5-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="603e5-108">Отчеты об истории профилей конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="603e5-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="603e5-109">Отчеты о сбоях регистрации.</span><span class="sxs-lookup"><span data-stu-id="603e5-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="603e5-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="603e5-110">Properties</span></span>
|<span data-ttu-id="603e5-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="603e5-111">Property</span></span>|<span data-ttu-id="603e5-112">Тип</span><span class="sxs-lookup"><span data-stu-id="603e5-112">Type</span></span>|<span data-ttu-id="603e5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="603e5-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="603e5-114">содержимое</span><span class="sxs-lookup"><span data-stu-id="603e5-114">content</span></span>|<span data-ttu-id="603e5-115">Поток</span><span class="sxs-lookup"><span data-stu-id="603e5-115">Stream</span></span>|<span data-ttu-id="603e5-116">Содержимое отчета; сведения зависят от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="603e5-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="603e5-117">Связи</span><span class="sxs-lookup"><span data-stu-id="603e5-117">Relationships</span></span>
<span data-ttu-id="603e5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="603e5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="603e5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="603e5-119">JSON Representation</span></span>
<span data-ttu-id="603e5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="603e5-120">Here is a JSON representation of the resource.</span></span>
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




