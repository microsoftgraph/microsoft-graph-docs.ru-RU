---
title: сложный тип Рекуесторманажер
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b2e3062383dd1cc1c7d04342b2dcbd5be0afd67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521126"
---
# <a name="requestomanager-complex-type"></a><span data-ttu-id="2de8f-103">сложный тип Рекуестоманажер</span><span class="sxs-lookup"><span data-stu-id="2de8f-103">requestoManager complex type</span></span>

<span data-ttu-id="2de8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2de8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2de8f-105">Используется в [параметрах утверждения политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2de8f-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="2de8f-106">Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение `#microsoft.graph.requestorManager` указывает на то, что руководитель запрашивающего пользователя должен быть утверждающим.</span><span class="sxs-lookup"><span data-stu-id="2de8f-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="2de8f-107">При создании этапа утверждения политики назначения пакетов Access с Рекуесторманажер также включает другой утверждающий, например одного пользователя или члена группы, если у запрашивающего пользователя нет руководителя.</span><span class="sxs-lookup"><span data-stu-id="2de8f-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="2de8f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2de8f-108">Properties</span></span>


| <span data-ttu-id="2de8f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2de8f-109">Property</span></span>                     | <span data-ttu-id="2de8f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2de8f-110">Type</span></span>                      | <span data-ttu-id="2de8f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2de8f-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="2de8f-112">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="2de8f-112">isBackup</span></span> | <span data-ttu-id="2de8f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="2de8f-113">Boolean</span></span> | <span data-ttu-id="2de8f-114">Для руководителя на этапе утверждения указывает, является ли руководитель резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="2de8f-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2de8f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2de8f-115">JSON representation</span></span>

<span data-ttu-id="2de8f-116">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2de8f-116">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
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
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
