---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователя, группы или организационной сущностей для контактов, при синхронизации локальных каталогов в Azure Active Directory.
ms.openlocfilehash: 9fa7850d39c9f7a490135a127938fc7fae30b6f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077456"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="92d55-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="92d55-103">onPremisesProvisioningError resource type</span></span>

> <span data-ttu-id="92d55-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="92d55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92d55-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92d55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92d55-106">Представляет ошибок синхронизации службы каталогов для объектов [пользователей](user.md), [группы](group.md)или [организации контакта](orgcontact.md) при синхронизации локальных каталогов в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="92d55-106">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="92d55-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="92d55-107">Properties</span></span>

| <span data-ttu-id="92d55-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="92d55-108">Property</span></span> | <span data-ttu-id="92d55-109">Тип</span><span class="sxs-lookup"><span data-stu-id="92d55-109">Type</span></span> | <span data-ttu-id="92d55-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92d55-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="92d55-111">category</span><span class="sxs-lookup"><span data-stu-id="92d55-111">category</span></span>|<span data-ttu-id="92d55-112">String</span><span class="sxs-lookup"><span data-stu-id="92d55-112">String</span></span>| <span data-ttu-id="92d55-113">Категория Ошибка подготовки.</span><span class="sxs-lookup"><span data-stu-id="92d55-113">Category of the provisioning error.</span></span> <span data-ttu-id="92d55-114">Примечание: В настоящее время доступно только один значений.</span><span class="sxs-lookup"><span data-stu-id="92d55-114">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="92d55-115">Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="92d55-115">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="92d55-116">Такое же значение для свойства содержат другие объекты.</span><span class="sxs-lookup"><span data-stu-id="92d55-116">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="92d55-117">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="92d55-117">occurredDateTime</span></span>|<span data-ttu-id="92d55-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d55-118">DateTimeOffset</span></span>| <span data-ttu-id="92d55-119">Дата и время, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="92d55-119">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="92d55-120">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="92d55-120">propertyCausingError</span></span>|<span data-ttu-id="92d55-121">String</span><span class="sxs-lookup"><span data-stu-id="92d55-121">String</span></span>| <span data-ttu-id="92d55-122">Имя свойства каталогов, вызывает ошибку.</span><span class="sxs-lookup"><span data-stu-id="92d55-122">Name of the directory property causing the error.</span></span> <span data-ttu-id="92d55-123">Текущий возможные значения: *UserPrincipalName* или *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="92d55-123">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="92d55-124">value</span><span class="sxs-lookup"><span data-stu-id="92d55-124">value</span></span>|<span data-ttu-id="92d55-125">String</span><span class="sxs-lookup"><span data-stu-id="92d55-125">String</span></span>| <span data-ttu-id="92d55-126">Значение свойства, вызывая ошибки.</span><span class="sxs-lookup"><span data-stu-id="92d55-126">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92d55-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92d55-127">JSON representation</span></span>
<span data-ttu-id="92d55-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92d55-128">Here is a JSON representation of the resource.</span></span>

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