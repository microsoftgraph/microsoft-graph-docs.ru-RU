---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для сущностей контактов пользователя, группы или организации при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 81586df0fac9b40fc11005b54139f2409af9604c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522223"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="87e35-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="87e35-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="87e35-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="87e35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87e35-105">Представляет ошибки синхронизации каталогов для сущностей контактов [пользователя](user.md), [группы](group.md)или [Организации](orgcontact.md) при синхронизации локальных каталогов с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="87e35-105">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="87e35-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="87e35-106">Properties</span></span>

| <span data-ttu-id="87e35-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="87e35-107">Property</span></span> | <span data-ttu-id="87e35-108">Тип</span><span class="sxs-lookup"><span data-stu-id="87e35-108">Type</span></span> | <span data-ttu-id="87e35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87e35-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="87e35-110">category</span><span class="sxs-lookup"><span data-stu-id="87e35-110">category</span></span>|<span data-ttu-id="87e35-111">String</span><span class="sxs-lookup"><span data-stu-id="87e35-111">String</span></span>| <span data-ttu-id="87e35-112">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="87e35-112">Category of the provisioning error.</span></span> <span data-ttu-id="87e35-113">Примечание. в настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="87e35-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="87e35-114">Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="87e35-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="87e35-115">Другие объекты содержат одно и то же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="87e35-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="87e35-116">оккурреддатетиме</span><span class="sxs-lookup"><span data-stu-id="87e35-116">occurredDateTime</span></span>|<span data-ttu-id="87e35-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e35-117">DateTimeOffset</span></span>| <span data-ttu-id="87e35-118">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="87e35-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="87e35-119">пропертикаусинжеррор</span><span class="sxs-lookup"><span data-stu-id="87e35-119">propertyCausingError</span></span>|<span data-ttu-id="87e35-120">String</span><span class="sxs-lookup"><span data-stu-id="87e35-120">String</span></span>| <span data-ttu-id="87e35-121">Имя свойства каталога, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="87e35-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="87e35-122">Текущие возможные значения: *userPrincipalName* или *proxyAddress*</span><span class="sxs-lookup"><span data-stu-id="87e35-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="87e35-123">value</span><span class="sxs-lookup"><span data-stu-id="87e35-123">value</span></span>|<span data-ttu-id="87e35-124">String</span><span class="sxs-lookup"><span data-stu-id="87e35-124">String</span></span>| <span data-ttu-id="87e35-125">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="87e35-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87e35-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87e35-126">JSON representation</span></span>
<span data-ttu-id="87e35-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87e35-127">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
