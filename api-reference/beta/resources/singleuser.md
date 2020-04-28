---
title: сложный тип SingleUser.
description: Определяет пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 13792bcffabbc9dceb272cd1cf156fbf9a5a5a10
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520571"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="d62d4-103">сложный тип SingleUser.</span><span class="sxs-lookup"><span data-stu-id="d62d4-103">singleUser complex type</span></span>

<span data-ttu-id="d62d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d62d4-105">Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d62d4-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="d62d4-106">Это `@odata.type` значение `#microsoft.graph.singleUser` указывает на то, что этот набор пользователей определяет определенного пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.</span><span class="sxs-lookup"><span data-stu-id="d62d4-106">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="d62d4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d62d4-107">Properties</span></span>

<span data-ttu-id="d62d4-108">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="d62d4-108">This type has the following properties:</span></span>

| <span data-ttu-id="d62d4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d62d4-109">Property</span></span>                     | <span data-ttu-id="d62d4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d62d4-110">Type</span></span>                      | <span data-ttu-id="d62d4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d62d4-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="d62d4-112">id</span><span class="sxs-lookup"><span data-stu-id="d62d4-112">id</span></span> |<span data-ttu-id="d62d4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d62d4-113">String</span></span> | <span data-ttu-id="d62d4-114">Идентификатор пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d62d4-114">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="d62d4-115">description</span><span class="sxs-lookup"><span data-stu-id="d62d4-115">description</span></span> |<span data-ttu-id="d62d4-116">String</span><span class="sxs-lookup"><span data-stu-id="d62d4-116">String</span></span> | <span data-ttu-id="d62d4-117">Имя пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d62d4-117">The name of the user in Azure AD.</span></span> <span data-ttu-id="d62d4-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d62d4-118">Read only.</span></span> |
| <span data-ttu-id="d62d4-119">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="d62d4-119">isBackup</span></span> | <span data-ttu-id="d62d4-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62d4-120">Boolean</span></span> | <span data-ttu-id="d62d4-121">Для **SingleUser.** на этапе утверждения указывает, является ли пользователь утверждающим резервной копии.</span><span class="sxs-lookup"><span data-stu-id="d62d4-121">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d62d4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d62d4-122">JSON representation</span></span>

<span data-ttu-id="d62d4-123">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d62d4-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "string (identifier)",
  "description": "string"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
