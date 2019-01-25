---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователя, группы или организационной сущностей для контактов, при синхронизации локальных каталогов в Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512733"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="66895-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="66895-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66895-104">Представляет ошибок синхронизации службы каталогов для объектов [пользователей](user.md), [группы](group.md)или [организации контакта](orgcontact.md) при синхронизации локальных каталогов в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66895-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="66895-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="66895-105">Properties</span></span>

| <span data-ttu-id="66895-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="66895-106">Property</span></span> | <span data-ttu-id="66895-107">Тип</span><span class="sxs-lookup"><span data-stu-id="66895-107">Type</span></span> | <span data-ttu-id="66895-108">Описание</span><span class="sxs-lookup"><span data-stu-id="66895-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="66895-109">category</span><span class="sxs-lookup"><span data-stu-id="66895-109">category</span></span>|<span data-ttu-id="66895-110">String</span><span class="sxs-lookup"><span data-stu-id="66895-110">String</span></span>| <span data-ttu-id="66895-111">Категория Ошибка подготовки.</span><span class="sxs-lookup"><span data-stu-id="66895-111">Category of the provisioning error.</span></span> <span data-ttu-id="66895-112">Примечание: В настоящее время доступно только один значений.</span><span class="sxs-lookup"><span data-stu-id="66895-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="66895-113">Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="66895-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="66895-114">Такое же значение для свойства содержат другие объекты.</span><span class="sxs-lookup"><span data-stu-id="66895-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="66895-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="66895-115">occurredDateTime</span></span>|<span data-ttu-id="66895-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66895-116">DateTimeOffset</span></span>| <span data-ttu-id="66895-117">Дата и время, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="66895-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="66895-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="66895-118">propertyCausingError</span></span>|<span data-ttu-id="66895-119">String</span><span class="sxs-lookup"><span data-stu-id="66895-119">String</span></span>| <span data-ttu-id="66895-120">Имя свойства каталогов, вызывает ошибку.</span><span class="sxs-lookup"><span data-stu-id="66895-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="66895-121">Текущий возможные значения: *UserPrincipalName* или *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="66895-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="66895-122">value</span><span class="sxs-lookup"><span data-stu-id="66895-122">value</span></span>|<span data-ttu-id="66895-123">Строка</span><span class="sxs-lookup"><span data-stu-id="66895-123">String</span></span>| <span data-ttu-id="66895-124">Значение свойства, вызывая ошибки.</span><span class="sxs-lookup"><span data-stu-id="66895-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66895-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66895-125">JSON representation</span></span>
<span data-ttu-id="66895-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66895-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
