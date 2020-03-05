---
title: Тип ресурса Хаспайлоадлинкресултитем
description: Класс, содержащий результат действия Хаспайлоадлинкс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 219bf9b1a2058b06895ec90883849cc8bdf0b569
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524008"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="fc190-103">Тип ресурса Хаспайлоадлинкресултитем</span><span class="sxs-lookup"><span data-stu-id="fc190-103">hasPayloadLinkResultItem resource type</span></span>

<span data-ttu-id="fc190-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc190-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc190-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc190-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc190-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc190-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc190-107">Класс, содержащий результат действия Хаспайлоадлинкс.</span><span class="sxs-lookup"><span data-stu-id="fc190-107">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="fc190-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc190-108">Properties</span></span>
|<span data-ttu-id="fc190-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc190-109">Property</span></span>|<span data-ttu-id="fc190-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fc190-110">Type</span></span>|<span data-ttu-id="fc190-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc190-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc190-112">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="fc190-112">payloadId</span></span>|<span data-ttu-id="fc190-113">String</span><span class="sxs-lookup"><span data-stu-id="fc190-113">String</span></span>|<span data-ttu-id="fc190-114">Ключ полезных данных в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="fc190-114">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="fc190-115">хаслинк</span><span class="sxs-lookup"><span data-stu-id="fc190-115">hasLink</span></span>|<span data-ttu-id="fc190-116">Логический</span><span class="sxs-lookup"><span data-stu-id="fc190-116">Boolean</span></span>|<span data-ttu-id="fc190-117">Указывает, содержит ли полезная нагрузка какую бы то ни было ссылку.</span><span class="sxs-lookup"><span data-stu-id="fc190-117">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="fc190-118">error</span><span class="sxs-lookup"><span data-stu-id="fc190-118">error</span></span>|<span data-ttu-id="fc190-119">String</span><span class="sxs-lookup"><span data-stu-id="fc190-119">String</span></span>|<span data-ttu-id="fc190-120">Сведения об исключении указывают на успешность проверки этого элемента. Пустая строка без ошибки.</span><span class="sxs-lookup"><span data-stu-id="fc190-120">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="fc190-121">sources</span><span class="sxs-lookup"><span data-stu-id="fc190-121">sources</span></span>|<span data-ttu-id="fc190-122">Коллекция [девицеандаппманажементассигнментсаурце](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="fc190-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="fc190-123">Причина, по которой получена ссылка.</span><span class="sxs-lookup"><span data-stu-id="fc190-123">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc190-124">Связи</span><span class="sxs-lookup"><span data-stu-id="fc190-124">Relationships</span></span>
<span data-ttu-id="fc190-125">Нет</span><span class="sxs-lookup"><span data-stu-id="fc190-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc190-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc190-126">JSON Representation</span></span>
<span data-ttu-id="fc190-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc190-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```



