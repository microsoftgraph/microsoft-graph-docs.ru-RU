---
title: Тип ресурса Обжектдефинитион
description: Описывает объект и его атрибуты. Определения объектов входят в состав Директоридефинитион, который обновляется в составе Синчронизатионсчема.
localization_priority: Normal
ms.openlocfilehash: d8182cad44deac156c077e977551abc9c31c7d25
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581767"
---
# <a name="objectdefinition-resource-type"></a><span data-ttu-id="4217d-104">Тип ресурса Обжектдефинитион</span><span class="sxs-lookup"><span data-stu-id="4217d-104">objectDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4217d-105">Описывает объект и его атрибуты.</span><span class="sxs-lookup"><span data-stu-id="4217d-105">Describes an object and its attributes.</span></span> <span data-ttu-id="4217d-106">Определения объектов входят в состав [директоридефинитион](synchronization-directorydefinition.md), который обновляется в составе [синчронизатионсчема](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="4217d-106">Object definitions are part of [directoryDefinition](synchronization-directorydefinition.md), which is updated as part of [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4217d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4217d-107">Properties</span></span>

| <span data-ttu-id="4217d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4217d-108">Property</span></span>      | <span data-ttu-id="4217d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4217d-109">Type</span></span>      | <span data-ttu-id="4217d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4217d-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4217d-111">attributes</span><span class="sxs-lookup"><span data-stu-id="4217d-111">attributes</span></span>     |<span data-ttu-id="4217d-112">Коллекция [аттрибутедефинитион](synchronization-attributedefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4217d-112">[attributeDefinition](synchronization-attributedefinition.md) collection</span></span>    | <span data-ttu-id="4217d-113">Определяет атрибуты объекта.</span><span class="sxs-lookup"><span data-stu-id="4217d-113">Defines attributes of the object.</span></span> |
|<span data-ttu-id="4217d-114">метаданных</span><span class="sxs-lookup"><span data-stu-id="4217d-114">metadata</span></span>       |<span data-ttu-id="4217d-115">Коллекция [метадатаентри](synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="4217d-115">[metadataEntry](synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="4217d-116">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="4217d-116">Additional extension properties.</span></span> <span data-ttu-id="4217d-117">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="4217d-117">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="4217d-118">name</span><span class="sxs-lookup"><span data-stu-id="4217d-118">name</span></span>           |<span data-ttu-id="4217d-119">String</span><span class="sxs-lookup"><span data-stu-id="4217d-119">String</span></span>     |<span data-ttu-id="4217d-120">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="4217d-120">Name of the object.</span></span> <span data-ttu-id="4217d-121">Должно быть уникальным в пределах определения каталога.</span><span class="sxs-lookup"><span data-stu-id="4217d-121">Must be unique within a directory definition.</span></span> <span data-ttu-id="4217d-122">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="4217d-122">Not nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4217d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4217d-123">JSON representation</span></span>

<span data-ttu-id="4217d-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4217d-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectDefinition"
}-->

```json
{
  "attributes": [{"@odata.type": "microsoft.graph.attributeDefinition"}],
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="4217d-125">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="4217d-125">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectDefinition"
}-->

```json
{
    "attributes": [
        {
            "anchor": true,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "objectId",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "IsSoftDeleted",
            "required": true,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "accountEnabled",
            "required": true,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "streetAddress",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "city",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "state",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "postalCode",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "country",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "companyName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "department",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "dirSyncEnabled",
            "required": false,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "displayName",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "extensionAttribute1",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "facsimileTelephoneNumber",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "givenName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "jobTitle",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mail",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mailNickname",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "manager",
            "required": false,
            "referencedObjects": [
                {
                    "referencedObjectName": "User",
                    "referencedProperty": null
                }
            ],
            "type": "Reference"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mobile",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "onPremisesSecurityIdentifier",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "originalUserPrincipalName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "passwordProfile.password",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "physicalDeliveryOfficeName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "preferredLanguage",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": true,
            "mutability": "ReadWrite",
            "name": "proxyAddresses",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "surname",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "telephoneNumber",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "userPrincipalName",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        }
    ],
    "metadata": [
        {
            "key": "IsSoftDeletionSupported",
            "value": "true"
        },
        {
            "key": "ConnectorDataStorageRequired",
            "value": "true"
        },
        {
            "key": "IsSynchronizeAllSupported",
            "value": "true"
        },
        {
            "key": "PropertyNameAccountEnabled",
            "value": "accountEnabled"
        },
        {
            "key": "PropertyNameSoftDeleted",
            "value": "IsSoftDeleted"
        }
    ],
    "name": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-objectdefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
