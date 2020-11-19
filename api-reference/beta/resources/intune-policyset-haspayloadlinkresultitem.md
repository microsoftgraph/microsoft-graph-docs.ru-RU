---
title: Тип ресурса Хаспайлоадлинкресултитем
description: Класс, содержащий результат действия Хаспайлоадлинкс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c6cc5e2f51265f062b6556438a177e4842e04e1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222480"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="4441e-103">Тип ресурса Хаспайлоадлинкресултитем</span><span class="sxs-lookup"><span data-stu-id="4441e-103">hasPayloadLinkResultItem resource type</span></span>

<span data-ttu-id="4441e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4441e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4441e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4441e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4441e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4441e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4441e-107">Класс, содержащий результат действия Хаспайлоадлинкс.</span><span class="sxs-lookup"><span data-stu-id="4441e-107">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="4441e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4441e-108">Properties</span></span>
|<span data-ttu-id="4441e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4441e-109">Property</span></span>|<span data-ttu-id="4441e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4441e-110">Type</span></span>|<span data-ttu-id="4441e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4441e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4441e-112">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="4441e-112">payloadId</span></span>|<span data-ttu-id="4441e-113">String</span><span class="sxs-lookup"><span data-stu-id="4441e-113">String</span></span>|<span data-ttu-id="4441e-114">Ключ полезных данных в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="4441e-114">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="4441e-115">хаслинк</span><span class="sxs-lookup"><span data-stu-id="4441e-115">hasLink</span></span>|<span data-ttu-id="4441e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4441e-116">Boolean</span></span>|<span data-ttu-id="4441e-117">Указывает, содержит ли полезная нагрузка какую бы то ни было ссылку.</span><span class="sxs-lookup"><span data-stu-id="4441e-117">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="4441e-118">error</span><span class="sxs-lookup"><span data-stu-id="4441e-118">error</span></span>|<span data-ttu-id="4441e-119">String</span><span class="sxs-lookup"><span data-stu-id="4441e-119">String</span></span>|<span data-ttu-id="4441e-120">Сведения об исключении указывают на успешность проверки этого элемента. Пустая строка без ошибки.</span><span class="sxs-lookup"><span data-stu-id="4441e-120">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="4441e-121">sources</span><span class="sxs-lookup"><span data-stu-id="4441e-121">sources</span></span>|<span data-ttu-id="4441e-122">Коллекция [девицеандаппманажементассигнментсаурце](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="4441e-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="4441e-123">Причина, по которой получена ссылка.</span><span class="sxs-lookup"><span data-stu-id="4441e-123">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4441e-124">Связи</span><span class="sxs-lookup"><span data-stu-id="4441e-124">Relationships</span></span>
<span data-ttu-id="4441e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="4441e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4441e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4441e-126">JSON Representation</span></span>
<span data-ttu-id="4441e-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4441e-127">Here is a JSON representation of the resource.</span></span>
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




