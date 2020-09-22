---
title: Тип ресурса Пассвордсинглесигнонфиелд
description: Поля для записи учетных данных для единого входа паролей
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d79f2347acabae0323e008a43adb7938d70d3768
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998196"
---
# <a name="passwordsinglesignonfield-resource-type"></a><span data-ttu-id="0b2c6-103">Тип ресурса Пассвордсинглесигнонфиелд</span><span class="sxs-lookup"><span data-stu-id="0b2c6-103">passwordSingleSignOnField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b2c6-104">Содержит поля для заполнения, используемые для заполнения учетных данных для единого входа на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="0b2c6-104">Contains the fields to capture to fill the use credentials for Password-based single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="0b2c6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b2c6-105">Properties</span></span>

| <span data-ttu-id="0b2c6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b2c6-106">Property</span></span>     | <span data-ttu-id="0b2c6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0b2c6-107">Type</span></span>        | <span data-ttu-id="0b2c6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0b2c6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b2c6-109">кустомизедлабел</span><span class="sxs-lookup"><span data-stu-id="0b2c6-109">customizedLabel</span></span>|<span data-ttu-id="0b2c6-110">String</span><span class="sxs-lookup"><span data-stu-id="0b2c6-110">String</span></span>|<span data-ttu-id="0b2c6-111">Переопределение названий и подписей для настройки.</span><span class="sxs-lookup"><span data-stu-id="0b2c6-111">Title/label override for customization.</span></span>|
|<span data-ttu-id="0b2c6-112">дефаултлабел</span><span class="sxs-lookup"><span data-stu-id="0b2c6-112">defaultLabel</span></span>|<span data-ttu-id="0b2c6-113">String</span><span class="sxs-lookup"><span data-stu-id="0b2c6-113">String</span></span>|<span data-ttu-id="0b2c6-114">Метка, которая будет использоваться, если Кустомизедлабел не указан.</span><span class="sxs-lookup"><span data-stu-id="0b2c6-114">Label that would be used if no customizedLabel is provided.</span></span> <span data-ttu-id="0b2c6-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b2c6-115">Read only.</span></span>|
|<span data-ttu-id="0b2c6-116">fieldId</span><span class="sxs-lookup"><span data-stu-id="0b2c6-116">fieldId</span></span>|<span data-ttu-id="0b2c6-117">String</span><span class="sxs-lookup"><span data-stu-id="0b2c6-117">String</span></span>|<span data-ttu-id="0b2c6-118">Идентификатор, используемый для идентификации типа поля.</span><span class="sxs-lookup"><span data-stu-id="0b2c6-118">Id used to identity the field type.</span></span> <span data-ttu-id="0b2c6-119">Это внутренний идентификатор, и возможные значения: `param_1` ,, `param_2` `param_userName` , `param_password` .</span><span class="sxs-lookup"><span data-stu-id="0b2c6-119">This is an internal id and possible values are `param_1`, `param_2`, `param_userName`, `param_password`.</span></span>|
|<span data-ttu-id="0b2c6-120">type</span><span class="sxs-lookup"><span data-stu-id="0b2c6-120">type</span></span>|<span data-ttu-id="0b2c6-121">String</span><span class="sxs-lookup"><span data-stu-id="0b2c6-121">String</span></span>|   <span data-ttu-id="0b2c6-122">Тип учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0b2c6-122">Type of the credential.</span></span> <span data-ttu-id="0b2c6-123">Возможные значения `text` : `password` .</span><span class="sxs-lookup"><span data-stu-id="0b2c6-123">The values can be `text`, `password`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b2c6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b2c6-124">JSON representation</span></span>

<span data-ttu-id="0b2c6-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b2c6-125">The following is a JSON representation of the resource.</span></span>

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

