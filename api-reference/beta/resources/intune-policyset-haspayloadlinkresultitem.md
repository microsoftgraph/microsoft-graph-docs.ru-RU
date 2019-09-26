---
title: Тип ресурса Хаспайлоадлинкресултитем
description: Класс, содержащий результат действия Хаспайлоадлинкс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 09e61f33151158c600e3a3ea783965f2f131fcce
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201268"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="7778b-103">Тип ресурса Хаспайлоадлинкресултитем</span><span class="sxs-lookup"><span data-stu-id="7778b-103">hasPayloadLinkResultItem resource type</span></span>

> <span data-ttu-id="7778b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7778b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7778b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7778b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7778b-106">Класс, содержащий результат действия Хаспайлоадлинкс.</span><span class="sxs-lookup"><span data-stu-id="7778b-106">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="7778b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7778b-107">Properties</span></span>
|<span data-ttu-id="7778b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7778b-108">Property</span></span>|<span data-ttu-id="7778b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7778b-109">Type</span></span>|<span data-ttu-id="7778b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7778b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7778b-111">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="7778b-111">payloadId</span></span>|<span data-ttu-id="7778b-112">String.</span><span class="sxs-lookup"><span data-stu-id="7778b-112">String</span></span>|<span data-ttu-id="7778b-113">Ключ полезных данных в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="7778b-113">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="7778b-114">хаслинк</span><span class="sxs-lookup"><span data-stu-id="7778b-114">hasLink</span></span>|<span data-ttu-id="7778b-115">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7778b-115">Boolean</span></span>|<span data-ttu-id="7778b-116">Указывает, содержит ли полезная нагрузка какую бы то ни было ссылку.</span><span class="sxs-lookup"><span data-stu-id="7778b-116">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="7778b-117">error</span><span class="sxs-lookup"><span data-stu-id="7778b-117">error</span></span>|<span data-ttu-id="7778b-118">String.</span><span class="sxs-lookup"><span data-stu-id="7778b-118">String</span></span>|<span data-ttu-id="7778b-119">Сведения об исключении указывают на успешность проверки этого элемента. Пустая строка без ошибки.</span><span class="sxs-lookup"><span data-stu-id="7778b-119">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="7778b-120">sources</span><span class="sxs-lookup"><span data-stu-id="7778b-120">sources</span></span>|<span data-ttu-id="7778b-121">Коллекция [девицеандаппманажементассигнментсаурце](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="7778b-121">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="7778b-122">Причина, по которой получена ссылка.</span><span class="sxs-lookup"><span data-stu-id="7778b-122">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7778b-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="7778b-123">Relationships</span></span>
<span data-ttu-id="7778b-124">Нет</span><span class="sxs-lookup"><span data-stu-id="7778b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7778b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7778b-125">JSON Representation</span></span>
<span data-ttu-id="7778b-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7778b-126">Here is a JSON representation of the resource.</span></span>
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



