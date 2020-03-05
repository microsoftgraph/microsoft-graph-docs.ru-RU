---
title: сложный тип Екстерналспонсорс
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03e73fe63e7624b2ab9d549c3b9ccd1526301a9c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498611"
---
# <a name="externalsponsors-complex-type"></a><span data-ttu-id="f0055-103">сложный тип Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="f0055-103">externalSponsors complex type</span></span>

<span data-ttu-id="f0055-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0055-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0055-105">Используется на этапе утверждения [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0055-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="f0055-106">Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение `#microsoft.graph.externalSponsors` указывает на то, что пользователь, подключенный к Организации, у которого есть внешние спонсоры, должен быть утверждающим.</span><span class="sxs-lookup"><span data-stu-id="f0055-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.externalSponsors` indicates that a requesting user's connected organization external sponsors are to be the approver.</span></span> <span data-ttu-id="f0055-107">Этот утверждающий применяется только к запросам пользователей, которые являются частью подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="f0055-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="f0055-108">При создании этапа утверждения политики назначения пакетов Access с Екстерналспонсорс также включает другой утверждающий, например одного пользователя или члена группы, если у подключенной Организации нет внешнего спонсора.</span><span class="sxs-lookup"><span data-stu-id="f0055-108">When creating an access package assignment policy approval stage with externalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an external sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="f0055-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0055-109">Properties</span></span>

| <span data-ttu-id="f0055-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0055-110">Property</span></span>                     | <span data-ttu-id="f0055-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f0055-111">Type</span></span>                      | <span data-ttu-id="f0055-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f0055-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="f0055-113">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="f0055-113">isBackup</span></span> | <span data-ttu-id="f0055-114">Логический</span><span class="sxs-lookup"><span data-stu-id="f0055-114">Boolean</span></span> | <span data-ttu-id="f0055-115">Указывает, является ли спонсор резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="f0055-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0055-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0055-116">JSON representation</span></span>

<span data-ttu-id="f0055-117">Ниже представлено представление этого типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0055-117">The following is a JSON representation of this type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.externalSponsors",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
