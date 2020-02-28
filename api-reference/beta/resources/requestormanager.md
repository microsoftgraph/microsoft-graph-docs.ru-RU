---
title: сложный тип Рекуесторманажер
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b7eea64e2d3f1d32b7ca60fc0c3a548401f7ef23
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331400"
---
# <a name="requestomanager-complex-type"></a><span data-ttu-id="d03a1-103">сложный тип Рекуестоманажер</span><span class="sxs-lookup"><span data-stu-id="d03a1-103">requestoManager complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d03a1-104">Используется в [параметрах утверждения политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d03a1-104">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="d03a1-105">Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение `#microsoft.graph.requestorManager` указывает на то, что руководитель запрашивающего пользователя должен быть утверждающим.</span><span class="sxs-lookup"><span data-stu-id="d03a1-105">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="d03a1-106">При создании этапа утверждения политики назначения пакетов Access с Рекуесторманажер также включает другой утверждающий, например одного пользователя или члена группы, если у запрашивающего пользователя нет руководителя.</span><span class="sxs-lookup"><span data-stu-id="d03a1-106">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="d03a1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d03a1-107">Properties</span></span>


| <span data-ttu-id="d03a1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d03a1-108">Property</span></span>                     | <span data-ttu-id="d03a1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d03a1-109">Type</span></span>                      | <span data-ttu-id="d03a1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d03a1-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="d03a1-111">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="d03a1-111">isBackup</span></span> | <span data-ttu-id="d03a1-112">Логический</span><span class="sxs-lookup"><span data-stu-id="d03a1-112">Boolean</span></span> | <span data-ttu-id="d03a1-113">Для руководителя на этапе утверждения указывает, является ли руководитель резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="d03a1-113">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d03a1-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d03a1-114">JSON representation</span></span>

<span data-ttu-id="d03a1-115">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d03a1-115">The following is a JSON representation of the type.</span></span>

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
