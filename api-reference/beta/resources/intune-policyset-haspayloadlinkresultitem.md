---
title: Тип ресурса Хаспайлоадлинкресултитем
description: Класс, содержащий результат действия Хаспайлоадлинкс.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 46568e386c2896db307f78cc12205c115605a76e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775908"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="dce66-103">Тип ресурса Хаспайлоадлинкресултитем</span><span class="sxs-lookup"><span data-stu-id="dce66-103">hasPayloadLinkResultItem resource type</span></span>

> <span data-ttu-id="dce66-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dce66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dce66-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dce66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dce66-106">Класс, содержащий результат действия Хаспайлоадлинкс.</span><span class="sxs-lookup"><span data-stu-id="dce66-106">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="dce66-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dce66-107">Properties</span></span>
|<span data-ttu-id="dce66-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dce66-108">Property</span></span>|<span data-ttu-id="dce66-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dce66-109">Type</span></span>|<span data-ttu-id="dce66-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dce66-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dce66-111">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="dce66-111">payloadId</span></span>|<span data-ttu-id="dce66-112">String</span><span class="sxs-lookup"><span data-stu-id="dce66-112">String</span></span>|<span data-ttu-id="dce66-113">Ключ полезных данных в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="dce66-113">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="dce66-114">хаслинк</span><span class="sxs-lookup"><span data-stu-id="dce66-114">hasLink</span></span>|<span data-ttu-id="dce66-115">Логический</span><span class="sxs-lookup"><span data-stu-id="dce66-115">Boolean</span></span>|<span data-ttu-id="dce66-116">Указывает, содержит ли полезная нагрузка какую бы то ни было ссылку.</span><span class="sxs-lookup"><span data-stu-id="dce66-116">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="dce66-117">error</span><span class="sxs-lookup"><span data-stu-id="dce66-117">error</span></span>|<span data-ttu-id="dce66-118">String</span><span class="sxs-lookup"><span data-stu-id="dce66-118">String</span></span>|<span data-ttu-id="dce66-119">Сведения об исключении указывают на успешность проверки этого элемента. Пустая строка без ошибки.</span><span class="sxs-lookup"><span data-stu-id="dce66-119">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="dce66-120">sources</span><span class="sxs-lookup"><span data-stu-id="dce66-120">sources</span></span>|<span data-ttu-id="dce66-121">Коллекция [девицеандаппманажементассигнментсаурце](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="dce66-121">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="dce66-122">Причина, по которой получена ссылка.</span><span class="sxs-lookup"><span data-stu-id="dce66-122">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dce66-123">Связи</span><span class="sxs-lookup"><span data-stu-id="dce66-123">Relationships</span></span>
<span data-ttu-id="dce66-124">Нет</span><span class="sxs-lookup"><span data-stu-id="dce66-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dce66-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dce66-125">JSON Representation</span></span>
<span data-ttu-id="dce66-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dce66-126">Here is a JSON representation of the resource.</span></span>
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



