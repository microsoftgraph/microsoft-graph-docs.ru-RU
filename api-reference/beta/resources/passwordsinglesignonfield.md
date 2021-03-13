---
title: тип ресурса passwordSingleSignOnField
description: Поля для захвата учетных данных для SSO пароля
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e0db6198d61715603acee54e7351c9fd5f2fed88
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761551"
---
# <a name="passwordsinglesignonfield-resource-type"></a><span data-ttu-id="0c5bc-103">тип ресурса passwordSingleSignOnField</span><span class="sxs-lookup"><span data-stu-id="0c5bc-103">passwordSingleSignOnField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c5bc-104">Содержит поля для захвата для заполнения учетных данных использования для одного входа на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="0c5bc-104">Contains the fields to capture to fill the use credentials for Password-based single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="0c5bc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c5bc-105">Properties</span></span>

| <span data-ttu-id="0c5bc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c5bc-106">Property</span></span>     | <span data-ttu-id="0c5bc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0c5bc-107">Type</span></span>        | <span data-ttu-id="0c5bc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5bc-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c5bc-109">customizedLabel</span><span class="sxs-lookup"><span data-stu-id="0c5bc-109">customizedLabel</span></span>|<span data-ttu-id="0c5bc-110">String</span><span class="sxs-lookup"><span data-stu-id="0c5bc-110">String</span></span>|<span data-ttu-id="0c5bc-111">Переопределение заголовка или метки для настройки.</span><span class="sxs-lookup"><span data-stu-id="0c5bc-111">Title/label override for customization.</span></span>|
|<span data-ttu-id="0c5bc-112">defaultLabel</span><span class="sxs-lookup"><span data-stu-id="0c5bc-112">defaultLabel</span></span>|<span data-ttu-id="0c5bc-113">String</span><span class="sxs-lookup"><span data-stu-id="0c5bc-113">String</span></span>|<span data-ttu-id="0c5bc-114">Метка, которая будет использоваться, если не будет предоставлена настройкаLabel.</span><span class="sxs-lookup"><span data-stu-id="0c5bc-114">Label that would be used if no customizedLabel is provided.</span></span> <span data-ttu-id="0c5bc-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c5bc-115">Read only.</span></span>|
|<span data-ttu-id="0c5bc-116">fieldId</span><span class="sxs-lookup"><span data-stu-id="0c5bc-116">fieldId</span></span>|<span data-ttu-id="0c5bc-117">String</span><span class="sxs-lookup"><span data-stu-id="0c5bc-117">String</span></span>|<span data-ttu-id="0c5bc-118">Идентификатор, используемый для удостоверения типа поля.</span><span class="sxs-lookup"><span data-stu-id="0c5bc-118">Id used to identity the field type.</span></span> <span data-ttu-id="0c5bc-119">Это внутренний id и возможные значения `param_1` , `param_2` , `param_userName` `param_password` .</span><span class="sxs-lookup"><span data-stu-id="0c5bc-119">This is an internal id and possible values are `param_1`, `param_2`, `param_userName`, `param_password`.</span></span>|
|<span data-ttu-id="0c5bc-120">type</span><span class="sxs-lookup"><span data-stu-id="0c5bc-120">type</span></span>|<span data-ttu-id="0c5bc-121">String</span><span class="sxs-lookup"><span data-stu-id="0c5bc-121">String</span></span>|   <span data-ttu-id="0c5bc-122">Тип учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0c5bc-122">Type of the credential.</span></span> <span data-ttu-id="0c5bc-123">Значения могут быть `text` , `password` .</span><span class="sxs-lookup"><span data-stu-id="0c5bc-123">The values can be `text`, `password`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c5bc-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c5bc-124">JSON representation</span></span>

<span data-ttu-id="0c5bc-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c5bc-125">The following is a JSON representation of the resource.</span></span>

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

