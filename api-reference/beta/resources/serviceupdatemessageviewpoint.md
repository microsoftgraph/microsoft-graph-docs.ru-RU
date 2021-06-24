---
title: тип ресурса serviceUpdateMessageViewpoint
description: Представляет данные точек представления пользователей для службыUpdateMessage".
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c84a07691c2507a9ff74102ac6f4b1675cb382e7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109223"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a><span data-ttu-id="1636c-103">тип ресурса serviceUpdateMessageViewpoint</span><span class="sxs-lookup"><span data-stu-id="1636c-103">serviceUpdateMessageViewpoint resource type</span></span>

<span data-ttu-id="1636c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1636c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1636c-105">Представляет данные точек представления пользователей для [службыUpdateMessage.](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="1636c-105">Represents user view points data for a [serviceUpdateMessage](../resources/serviceupdatemessage.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1636c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1636c-106">Properties</span></span>
|<span data-ttu-id="1636c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1636c-107">Property</span></span>|<span data-ttu-id="1636c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1636c-108">Type</span></span>|<span data-ttu-id="1636c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1636c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1636c-110">isArchived</span><span class="sxs-lookup"><span data-stu-id="1636c-110">isArchived</span></span>|<span data-ttu-id="1636c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1636c-111">Boolean</span></span>|<span data-ttu-id="1636c-112">Указывает, архивировать ли сообщение пользователь.</span><span class="sxs-lookup"><span data-stu-id="1636c-112">Indicates whether the user archived the message.</span></span>|
|<span data-ttu-id="1636c-113">isFavorited</span><span class="sxs-lookup"><span data-stu-id="1636c-113">isFavorited</span></span>|<span data-ttu-id="1636c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1636c-114">Boolean</span></span>|<span data-ttu-id="1636c-115">Указывает, отметил ли пользователь сообщение как избранное.</span><span class="sxs-lookup"><span data-stu-id="1636c-115">Indicates whether the user marked the message as favorite.</span></span>|
|<span data-ttu-id="1636c-116">isRead</span><span class="sxs-lookup"><span data-stu-id="1636c-116">isRead</span></span>|<span data-ttu-id="1636c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1636c-117">Boolean</span></span>|<span data-ttu-id="1636c-118">Указывает, читал ли пользователь сообщение.</span><span class="sxs-lookup"><span data-stu-id="1636c-118">Indicates whether the user read the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1636c-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="1636c-119">Relationships</span></span>
<span data-ttu-id="1636c-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1636c-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1636c-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1636c-121">JSON representation</span></span>
<span data-ttu-id="1636c-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1636c-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessageViewpoint",
  "isRead": "Boolean",
  "isArchived": "Boolean",
  "isFavorited": "Boolean"
}
```