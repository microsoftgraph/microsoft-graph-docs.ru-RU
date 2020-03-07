---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для группы пользователей и контактных ресурсов при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f11058bc75d6e5e417813b8b257f3a7ff78e94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534150"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="b3fe4-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="b3fe4-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="b3fe4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3fe4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3fe4-105">Представляет ошибки синхронизации каталогов для [пользователей](user.md), [групп](group.md) и [orgContact](orgcontact.md) ресурсов при синхронизации локальных каталогов с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="b3fe4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3fe4-106">Properties</span></span>

| <span data-ttu-id="b3fe4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3fe4-107">Property</span></span> | <span data-ttu-id="b3fe4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b3fe4-108">Type</span></span> | <span data-ttu-id="b3fe4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b3fe4-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b3fe4-110">category</span><span class="sxs-lookup"><span data-stu-id="b3fe4-110">category</span></span>|<span data-ttu-id="b3fe4-111">String</span><span class="sxs-lookup"><span data-stu-id="b3fe4-111">String</span></span>| <span data-ttu-id="b3fe4-112">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-112">Category of the provisioning error.</span></span> <span data-ttu-id="b3fe4-113">Примечание. в настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="b3fe4-114">Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="b3fe4-115">Другие объекты содержат одно и то же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="b3fe4-116">оккурреддатетиме</span><span class="sxs-lookup"><span data-stu-id="b3fe4-116">occurredDateTime</span></span>|<span data-ttu-id="b3fe4-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fe4-117">DateTimeOffset</span></span>| <span data-ttu-id="b3fe4-118">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="b3fe4-119">пропертикаусинжеррор</span><span class="sxs-lookup"><span data-stu-id="b3fe4-119">propertyCausingError</span></span>|<span data-ttu-id="b3fe4-120">Строка</span><span class="sxs-lookup"><span data-stu-id="b3fe4-120">String</span></span>| <span data-ttu-id="b3fe4-121">Имя свойства каталога, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="b3fe4-122">Текущие возможные значения: *userPrincipalName* или *proxyAddress*</span><span class="sxs-lookup"><span data-stu-id="b3fe4-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="b3fe4-123">value</span><span class="sxs-lookup"><span data-stu-id="b3fe4-123">value</span></span>|<span data-ttu-id="b3fe4-124">String</span><span class="sxs-lookup"><span data-stu-id="b3fe4-124">String</span></span>| <span data-ttu-id="b3fe4-125">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b3fe4-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3fe4-126">JSON representation</span></span>
<span data-ttu-id="b3fe4-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3fe4-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
