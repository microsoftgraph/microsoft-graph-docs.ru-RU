---
title: сложный тип Рекуесторманажер
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca8559d3ecf7ba4110a7e2871f8e6acf545d2906
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581154"
---
# <a name="requestormanager-complex-type"></a><span data-ttu-id="3c1c9-103">сложный тип Рекуесторманажер</span><span class="sxs-lookup"><span data-stu-id="3c1c9-103">requestorManager complex type</span></span>

<span data-ttu-id="3c1c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c1c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c1c9-105">Используется в [параметрах утверждения политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c1c9-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="3c1c9-106">Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение указывает на то `#microsoft.graph.requestorManager` , что руководитель запрашивающего пользователя должен быть утверждающим.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="3c1c9-107">При создании этапа утверждения политики назначения пакетов Access с Рекуесторманажер также включает другой утверждающий, например одного пользователя или члена группы, если у запрашивающего пользователя нет руководителя.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="3c1c9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c1c9-108">Properties</span></span>


| <span data-ttu-id="3c1c9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c1c9-109">Property</span></span>                     | <span data-ttu-id="3c1c9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3c1c9-110">Type</span></span>                      | <span data-ttu-id="3c1c9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c1c9-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="3c1c9-112">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="3c1c9-112">isBackup</span></span> | <span data-ttu-id="3c1c9-113">Логический</span><span class="sxs-lookup"><span data-stu-id="3c1c9-113">Boolean</span></span> | <span data-ttu-id="3c1c9-114">Для руководителя на этапе утверждения указывает, является ли руководитель резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |
|<span data-ttu-id="3c1c9-115">манажерлевел</span><span class="sxs-lookup"><span data-stu-id="3c1c9-115">managerLevel</span></span> | <span data-ttu-id="3c1c9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3c1c9-116">Int32</span></span> | <span data-ttu-id="3c1c9-117">Иерархический уровень руководителя по отношению к запрашивающему.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-117">The hierarchical level of the manager with respect to the requestor.</span></span> <span data-ttu-id="3c1c9-118">Например, непосредственный менеджер запрашивающего Манажерлевел должен иметь значение 1, в то время как руководитель запрашивающего менеджера будет иметь Манажерлевел 2.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-118">For example, the direct manager of a requestor would have a managerLevel of 1, while the manager of the requestor's manager would have a managerLevel of 2.</span></span> <span data-ttu-id="3c1c9-119">Значение по умолчанию для Манажерлевел — 1.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-119">Default value for managerLevel is 1.</span></span> <span data-ttu-id="3c1c9-120">Возможные значения этого свойства находятся в диапазоне от 1 до 2.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-120">Possible values for this property range from 1 to 2.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3c1c9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c1c9-121">JSON representation</span></span>

<span data-ttu-id="3c1c9-122">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c1c9-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
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


