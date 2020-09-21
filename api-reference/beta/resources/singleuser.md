---
title: сложный тип SingleUser.
description: Определяет пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb6b665814281629836f4c5148b567de776ef2ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067127"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="aafe3-103">сложный тип SingleUser.</span><span class="sxs-lookup"><span data-stu-id="aafe3-103">singleUser complex type</span></span>

<span data-ttu-id="aafe3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aafe3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aafe3-105">Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aafe3-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="aafe3-106">`@odata.type`Это значение `#microsoft.graph.singleUser` указывает на то, что этот набор пользователей определяет определенного пользователя в клиенте, который будет разрешен в качестве запрашивающего, утверждающего или проверяющего.</span><span class="sxs-lookup"><span data-stu-id="aafe3-106">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="aafe3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aafe3-107">Properties</span></span>

<span data-ttu-id="aafe3-108">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="aafe3-108">This type has the following properties:</span></span>

| <span data-ttu-id="aafe3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aafe3-109">Property</span></span>                     | <span data-ttu-id="aafe3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aafe3-110">Type</span></span>                      | <span data-ttu-id="aafe3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aafe3-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="aafe3-112">id</span><span class="sxs-lookup"><span data-stu-id="aafe3-112">id</span></span> |<span data-ttu-id="aafe3-113">String</span><span class="sxs-lookup"><span data-stu-id="aafe3-113">String</span></span> | <span data-ttu-id="aafe3-114">Идентификатор пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aafe3-114">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="aafe3-115">description</span><span class="sxs-lookup"><span data-stu-id="aafe3-115">description</span></span> |<span data-ttu-id="aafe3-116">String</span><span class="sxs-lookup"><span data-stu-id="aafe3-116">String</span></span> | <span data-ttu-id="aafe3-117">Имя пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aafe3-117">The name of the user in Azure AD.</span></span> <span data-ttu-id="aafe3-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aafe3-118">Read only.</span></span> |
| <span data-ttu-id="aafe3-119">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="aafe3-119">isBackup</span></span> | <span data-ttu-id="aafe3-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="aafe3-120">Boolean</span></span> | <span data-ttu-id="aafe3-121">Для **SingleUser.** на этапе утверждения указывает, является ли пользователь утверждающим резервной копии.</span><span class="sxs-lookup"><span data-stu-id="aafe3-121">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aafe3-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aafe3-122">JSON representation</span></span>

<span data-ttu-id="aafe3-123">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aafe3-123">The following is a JSON representation of the type.</span></span>

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


