---
title: Тип ресурса Пассвордсинглесигнонфиелд
description: Поля для записи учетных данных для единого входа паролей
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e20bcd2b9ddeab5ce255285fb6e13af5acb72fce
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658190"
---
# <a name="passwordsinglesignonfield-resource-type"></a><span data-ttu-id="11b72-103">Тип ресурса Пассвордсинглесигнонфиелд</span><span class="sxs-lookup"><span data-stu-id="11b72-103">passwordSingleSignOnField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11b72-104">Содержит поля для заполнения, используемые для заполнения учетных данных для единого входа на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="11b72-104">Contains the fields to capture to fill the use credentials for Password-based single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="11b72-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="11b72-105">Properties</span></span>

| <span data-ttu-id="11b72-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="11b72-106">Property</span></span>     | <span data-ttu-id="11b72-107">Тип</span><span class="sxs-lookup"><span data-stu-id="11b72-107">Type</span></span>        | <span data-ttu-id="11b72-108">Описание</span><span class="sxs-lookup"><span data-stu-id="11b72-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11b72-109">кустомизедлабел</span><span class="sxs-lookup"><span data-stu-id="11b72-109">customizedLabel</span></span>|<span data-ttu-id="11b72-110">String</span><span class="sxs-lookup"><span data-stu-id="11b72-110">String</span></span>|<span data-ttu-id="11b72-111">Переопределение названий и подписей для настройки.</span><span class="sxs-lookup"><span data-stu-id="11b72-111">Title/label override for customization.</span></span>|
|<span data-ttu-id="11b72-112">дефаултлабел</span><span class="sxs-lookup"><span data-stu-id="11b72-112">defaultLabel</span></span>|<span data-ttu-id="11b72-113">String</span><span class="sxs-lookup"><span data-stu-id="11b72-113">String</span></span>|<span data-ttu-id="11b72-114">Метка, которая будет использоваться, если Кустомизедлабел не указан.</span><span class="sxs-lookup"><span data-stu-id="11b72-114">Label that would be used if no customizedLabel is provided.</span></span> <span data-ttu-id="11b72-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11b72-115">Read only.</span></span>|
|<span data-ttu-id="11b72-116">fieldId</span><span class="sxs-lookup"><span data-stu-id="11b72-116">fieldId</span></span>|<span data-ttu-id="11b72-117">String</span><span class="sxs-lookup"><span data-stu-id="11b72-117">String</span></span>|<span data-ttu-id="11b72-118">Идентификатор, используемый для идентификации типа поля.</span><span class="sxs-lookup"><span data-stu-id="11b72-118">Id used to identity the field type.</span></span> <span data-ttu-id="11b72-119">Это внутренний идентификатор, и возможные значения: `param_1` ,, `param_2` `param_userName` , `param_password` .</span><span class="sxs-lookup"><span data-stu-id="11b72-119">This is an internal id and possible values are `param_1`, `param_2`, `param_userName`, `param_password`.</span></span>|
|<span data-ttu-id="11b72-120">type</span><span class="sxs-lookup"><span data-stu-id="11b72-120">type</span></span>|<span data-ttu-id="11b72-121">String</span><span class="sxs-lookup"><span data-stu-id="11b72-121">String</span></span>|   <span data-ttu-id="11b72-122">Тип учетных данных.</span><span class="sxs-lookup"><span data-stu-id="11b72-122">Type of the credential.</span></span> <span data-ttu-id="11b72-123">Возможные значения `text` : `password` .</span><span class="sxs-lookup"><span data-stu-id="11b72-123">The values can be `text`, `password`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11b72-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11b72-124">JSON representation</span></span>

<span data-ttu-id="11b72-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11b72-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnField",
  "baseType": null
}-->

```json
{
  "customizedLabel": "String",
  "defaultLabel": "String",
  "fieldId": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->