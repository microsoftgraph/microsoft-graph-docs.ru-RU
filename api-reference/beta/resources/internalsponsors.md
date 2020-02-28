---
title: сложный тип Интерналспонсорс
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c7ec468638de5e9a49cbf2f664eb7d05e3bef5b1
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331480"
---
# <a name="internalsponsors-complex-type"></a><span data-ttu-id="62281-103">сложный тип Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="62281-103">internalSponsors complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62281-104">Используется на этапе утверждения [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62281-104">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="62281-105">Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение `#microsoft.graph.internalSponsors` указывает на то, что пользователь, подключенный к Организации, может быть утверждающим в качестве внутреннего спонсора.</span><span class="sxs-lookup"><span data-stu-id="62281-105">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.internalSponsors` indicates that a requesting user's connected organization internal sponsors are to be the approver.</span></span> <span data-ttu-id="62281-106">Этот утверждающий применяется только к запросам пользователей, которые являются частью подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="62281-106">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="62281-107">При создании этапа утверждения политики назначения пакетов Access с Интерналспонсорс также включает другой утверждающий, например одного пользователя или члена группы, если у подключенной Организации нет внутреннего спонсора.</span><span class="sxs-lookup"><span data-stu-id="62281-107">When creating an access package assignment policy approval stage with internalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an internal sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="62281-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="62281-108">Properties</span></span>

| <span data-ttu-id="62281-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="62281-109">Property</span></span>                     | <span data-ttu-id="62281-110">Тип</span><span class="sxs-lookup"><span data-stu-id="62281-110">Type</span></span>                      | <span data-ttu-id="62281-111">Описание</span><span class="sxs-lookup"><span data-stu-id="62281-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="62281-112">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="62281-112">isBackup</span></span> | <span data-ttu-id="62281-113">Логический</span><span class="sxs-lookup"><span data-stu-id="62281-113">Boolean</span></span> | <span data-ttu-id="62281-114">Указывает, является ли спонсор резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="62281-114">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62281-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62281-115">JSON representation</span></span>

<span data-ttu-id="62281-116">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62281-116">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.internalSponsors",
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
