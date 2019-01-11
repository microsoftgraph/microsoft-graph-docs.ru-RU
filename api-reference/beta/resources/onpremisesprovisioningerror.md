---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователя, группы или организационной сущностей для контактов, при синхронизации локальных каталогов в Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 1ea9efcd4d9db5cf7cc5b8f0a18b35345d06c3fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817740"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="ae8d1-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="ae8d1-103">onPremisesProvisioningError resource type</span></span>

> <span data-ttu-id="ae8d1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae8d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae8d1-106">Представляет ошибок синхронизации службы каталогов для объектов [пользователей](user.md), [группы](group.md)или [организации контакта](orgcontact.md) при синхронизации локальных каталогов в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-106">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="ae8d1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae8d1-107">Properties</span></span>

| <span data-ttu-id="ae8d1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae8d1-108">Property</span></span> | <span data-ttu-id="ae8d1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ae8d1-109">Type</span></span> | <span data-ttu-id="ae8d1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ae8d1-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ae8d1-111">category</span><span class="sxs-lookup"><span data-stu-id="ae8d1-111">category</span></span>|<span data-ttu-id="ae8d1-112">String</span><span class="sxs-lookup"><span data-stu-id="ae8d1-112">String</span></span>| <span data-ttu-id="ae8d1-113">Категория Ошибка подготовки.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-113">Category of the provisioning error.</span></span> <span data-ttu-id="ae8d1-114">Примечание: В настоящее время доступно только один значений.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-114">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="ae8d1-115">Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-115">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="ae8d1-116">Такое же значение для свойства содержат другие объекты.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-116">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="ae8d1-117">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="ae8d1-117">occurredDateTime</span></span>|<span data-ttu-id="ae8d1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae8d1-118">DateTimeOffset</span></span>| <span data-ttu-id="ae8d1-119">Дата и время, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-119">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="ae8d1-120">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="ae8d1-120">propertyCausingError</span></span>|<span data-ttu-id="ae8d1-121">Строка</span><span class="sxs-lookup"><span data-stu-id="ae8d1-121">String</span></span>| <span data-ttu-id="ae8d1-122">Имя свойства каталогов, вызывает ошибку.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-122">Name of the directory property causing the error.</span></span> <span data-ttu-id="ae8d1-123">Текущий возможные значения: *UserPrincipalName* или *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="ae8d1-123">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="ae8d1-124">value</span><span class="sxs-lookup"><span data-stu-id="ae8d1-124">value</span></span>|<span data-ttu-id="ae8d1-125">Строка</span><span class="sxs-lookup"><span data-stu-id="ae8d1-125">String</span></span>| <span data-ttu-id="ae8d1-126">Значение свойства, вызывая ошибки.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-126">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae8d1-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae8d1-127">JSON representation</span></span>
<span data-ttu-id="ae8d1-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae8d1-128">Here is a JSON representation of the resource.</span></span>

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
