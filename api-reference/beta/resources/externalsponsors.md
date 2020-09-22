---
title: сложный тип Екстерналспонсорс
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4db88b74ae0acb2e817bd575f4e990774533064e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013702"
---
# <a name="externalsponsors-complex-type"></a><span data-ttu-id="74672-103">сложный тип Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="74672-103">externalSponsors complex type</span></span>

<span data-ttu-id="74672-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74672-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74672-105">Используется на этапе утверждения [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74672-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="74672-106">Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение `#microsoft.graph.externalSponsors` указывает на то, что пользователь, подключенный к Организации, у которого есть внешние спонсоры, должен быть утверждающим.</span><span class="sxs-lookup"><span data-stu-id="74672-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.externalSponsors` indicates that a requesting user's connected organization external sponsors are to be the approver.</span></span> <span data-ttu-id="74672-107">Этот утверждающий применяется только к запросам пользователей, которые являются частью подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="74672-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="74672-108">При создании этапа утверждения политики назначения пакетов Access с Екстерналспонсорс также включает другой утверждающий, например одного пользователя или члена группы, если у подключенной Организации нет внешнего спонсора.</span><span class="sxs-lookup"><span data-stu-id="74672-108">When creating an access package assignment policy approval stage with externalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an external sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="74672-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="74672-109">Properties</span></span>

| <span data-ttu-id="74672-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="74672-110">Property</span></span>                     | <span data-ttu-id="74672-111">Тип</span><span class="sxs-lookup"><span data-stu-id="74672-111">Type</span></span>                      | <span data-ttu-id="74672-112">Описание</span><span class="sxs-lookup"><span data-stu-id="74672-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="74672-113">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="74672-113">isBackup</span></span> | <span data-ttu-id="74672-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="74672-114">Boolean</span></span> | <span data-ttu-id="74672-115">Указывает, является ли спонсор резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="74672-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74672-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74672-116">JSON representation</span></span>

<span data-ttu-id="74672-117">Ниже представлено представление этого типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74672-117">The following is a JSON representation of this type.</span></span>

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


