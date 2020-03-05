---
title: сложный тип User
description: Абстрактный базовый тип для типов, используемых в параметрах просмотра запроса, утверждения и назначения для политики назначения пакетов Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 77f0f990587531c10914644366e066a0fd659f37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519507"
---
# <a name="userset-complex-type"></a><span data-ttu-id="f3f45-103">сложный тип User</span><span class="sxs-lookup"><span data-stu-id="f3f45-103">userSet complex type</span></span>

<span data-ttu-id="f3f45-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f3f45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3f45-105">Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f3f45-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="f3f45-106">Абстрактный базовый тип для типов [SingleUser.](singleuser.md),[граупмемберс](groupmembers.md), [коннектедорганизатионмемберс](connectedorganizationmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md)и [екстерналспонсорс](externalsponsors.md) .</span><span class="sxs-lookup"><span data-stu-id="f3f45-106">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="f3f45-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3f45-107">Properties</span></span>

| <span data-ttu-id="f3f45-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3f45-108">Property</span></span>                     | <span data-ttu-id="f3f45-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3f45-109">Type</span></span>                      | <span data-ttu-id="f3f45-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3f45-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="f3f45-111">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="f3f45-111">isBackup</span></span> | <span data-ttu-id="f3f45-112">Логический</span><span class="sxs-lookup"><span data-stu-id="f3f45-112">Boolean</span></span> | <span data-ttu-id="f3f45-113">Для пользователя на этапе утверждения данное свойство указывает, является ли пользователь утверждающим резервной копии.</span><span class="sxs-lookup"><span data-stu-id="f3f45-113">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3f45-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3f45-114">JSON representation</span></span>

<span data-ttu-id="f3f45-115">Ниже представлено представление объекта User в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3f45-115">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="f3f45-116">Обратите внимание, что пользовательский набор является абстрактным базовым классом, и поэтому не может быть отправлен или получен.</span><span class="sxs-lookup"><span data-stu-id="f3f45-116">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="f3f45-117">Вместо этого используется один из `@odata.type` "`#microsoft.graph.singleUser``#microsoft.graph.groupMembers`", "", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" или "`#microsoft.graph.externalSponsors`".</span><span class="sxs-lookup"><span data-stu-id="f3f45-117">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

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
