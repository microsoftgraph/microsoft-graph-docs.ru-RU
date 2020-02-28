---
title: сложный тип User
description: Абстрактный базовый тип для типов, используемых в параметрах просмотра запроса, утверждения и назначения для политики назначения пакетов Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f23953b30918dec40f37f7809c7c024167c34132
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331484"
---
# <a name="userset-complex-type"></a><span data-ttu-id="e436a-103">сложный тип User</span><span class="sxs-lookup"><span data-stu-id="e436a-103">userSet complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e436a-104">Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e436a-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="e436a-105">Абстрактный базовый тип для типов [SingleUser.](singleuser.md),[граупмемберс](groupmembers.md), [коннектедорганизатионмемберс](connectedorganizationmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md)и [екстерналспонсорс](externalsponsors.md) .</span><span class="sxs-lookup"><span data-stu-id="e436a-105">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="e436a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e436a-106">Properties</span></span>

| <span data-ttu-id="e436a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e436a-107">Property</span></span>                     | <span data-ttu-id="e436a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e436a-108">Type</span></span>                      | <span data-ttu-id="e436a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e436a-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="e436a-110">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="e436a-110">isBackup</span></span> | <span data-ttu-id="e436a-111">Логический</span><span class="sxs-lookup"><span data-stu-id="e436a-111">Boolean</span></span> | <span data-ttu-id="e436a-112">Для пользователя на этапе утверждения данное свойство указывает, является ли пользователь утверждающим резервной копии.</span><span class="sxs-lookup"><span data-stu-id="e436a-112">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e436a-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e436a-113">JSON representation</span></span>

<span data-ttu-id="e436a-114">Ниже представлено представление объекта User в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e436a-114">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="e436a-115">Обратите внимание, что пользовательский набор является абстрактным базовым классом, и поэтому не может быть отправлен или получен.</span><span class="sxs-lookup"><span data-stu-id="e436a-115">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="e436a-116">Вместо этого используется один из `@odata.type` "`#microsoft.graph.singleUser``#microsoft.graph.groupMembers`", "", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" или "`#microsoft.graph.externalSponsors`".</span><span class="sxs-lookup"><span data-stu-id="e436a-116">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet",
  "baseType": ""
}-->

```json
{
       "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
