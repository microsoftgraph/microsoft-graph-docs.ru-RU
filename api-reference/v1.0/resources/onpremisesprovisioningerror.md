---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для группы пользователей и контактных ресурсов при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e170fa0e86cfb6ebfcdf63b371c6a67bb8766b80
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468341"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="6cbf6-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="6cbf6-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="6cbf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cbf6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cbf6-105">Представляет ошибки синхронизации каталогов для [пользователей](user.md), [групп](group.md) и [orgContact](orgcontact.md) ресурсов при синхронизации локальных каталогов с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="6cbf6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6cbf6-106">Properties</span></span>

| <span data-ttu-id="6cbf6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cbf6-107">Property</span></span> | <span data-ttu-id="6cbf6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6cbf6-108">Type</span></span> | <span data-ttu-id="6cbf6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6cbf6-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6cbf6-110">category</span><span class="sxs-lookup"><span data-stu-id="6cbf6-110">category</span></span>|<span data-ttu-id="6cbf6-111">String</span><span class="sxs-lookup"><span data-stu-id="6cbf6-111">String</span></span>| <span data-ttu-id="6cbf6-112">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-112">Category of the provisioning error.</span></span> <span data-ttu-id="6cbf6-113">Примечание. в настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="6cbf6-114">Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="6cbf6-115">Другие объекты содержат одно и то же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="6cbf6-116">оккурреддатетиме</span><span class="sxs-lookup"><span data-stu-id="6cbf6-116">occurredDateTime</span></span>|<span data-ttu-id="6cbf6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cbf6-117">DateTimeOffset</span></span>| <span data-ttu-id="6cbf6-118">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="6cbf6-119">пропертикаусинжеррор</span><span class="sxs-lookup"><span data-stu-id="6cbf6-119">propertyCausingError</span></span>|<span data-ttu-id="6cbf6-120">String</span><span class="sxs-lookup"><span data-stu-id="6cbf6-120">String</span></span>| <span data-ttu-id="6cbf6-121">Имя свойства каталога, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="6cbf6-122">Текущие возможные значения: *userPrincipalName* или *proxyAddress*</span><span class="sxs-lookup"><span data-stu-id="6cbf6-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="6cbf6-123">value</span><span class="sxs-lookup"><span data-stu-id="6cbf6-123">value</span></span>|<span data-ttu-id="6cbf6-124">String</span><span class="sxs-lookup"><span data-stu-id="6cbf6-124">String</span></span>| <span data-ttu-id="6cbf6-125">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6cbf6-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6cbf6-126">JSON representation</span></span>
<span data-ttu-id="6cbf6-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cbf6-127">Here is a JSON representation of the resource.</span></span>

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
