---
title: сложный тип SingleUser.
description: Определяет пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d4db47278051dd79b697dc352549b95b872e4aa
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331406"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="ff477-103">сложный тип SingleUser.</span><span class="sxs-lookup"><span data-stu-id="ff477-103">singleUser complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff477-104">Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ff477-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="ff477-105">Это `@odata.type` значение `#microsoft.graph.singleUser` указывает на то, что этот набор пользователей определяет определенного пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.</span><span class="sxs-lookup"><span data-stu-id="ff477-105">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="ff477-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff477-106">Properties</span></span>

<span data-ttu-id="ff477-107">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="ff477-107">This type has the following properties:</span></span>

| <span data-ttu-id="ff477-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff477-108">Property</span></span>                     | <span data-ttu-id="ff477-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff477-109">Type</span></span>                      | <span data-ttu-id="ff477-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff477-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="ff477-111">id</span><span class="sxs-lookup"><span data-stu-id="ff477-111">id</span></span> |<span data-ttu-id="ff477-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ff477-112">String</span></span> | <span data-ttu-id="ff477-113">Идентификатор пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ff477-113">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="ff477-114">description</span><span class="sxs-lookup"><span data-stu-id="ff477-114">description</span></span> |<span data-ttu-id="ff477-115">String</span><span class="sxs-lookup"><span data-stu-id="ff477-115">String</span></span> | <span data-ttu-id="ff477-116">Имя пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ff477-116">The name of the user in Azure AD.</span></span> <span data-ttu-id="ff477-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff477-117">Read only.</span></span> |
| <span data-ttu-id="ff477-118">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="ff477-118">isBackup</span></span> | <span data-ttu-id="ff477-119">Логический</span><span class="sxs-lookup"><span data-stu-id="ff477-119">Boolean</span></span> | <span data-ttu-id="ff477-120">Для **SingleUser.** на этапе утверждения указывает, является ли пользователь утверждающим резервной копии.</span><span class="sxs-lookup"><span data-stu-id="ff477-120">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff477-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff477-121">JSON representation</span></span>

<span data-ttu-id="ff477-122">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff477-122">The following is a JSON representation of the type.</span></span>

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
