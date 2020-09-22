---
title: Тип ресурса Credential
description: Указывает одну учетную запись, используемую для входа в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a281e39850ea18ee3bcbe0d83c5df3b41d0ccd31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016690"
---
# <a name="credential-resource-type"></a><span data-ttu-id="00d7f-103">Тип ресурса Credential</span><span class="sxs-lookup"><span data-stu-id="00d7f-103">credential resource type</span></span>

<span data-ttu-id="00d7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00d7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00d7f-105">Указывает одну учетную запись, используемую для входа в приложение.</span><span class="sxs-lookup"><span data-stu-id="00d7f-105">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="00d7f-106">Например, username это один учетный набор учетных данных, пароль — это еще одна учетная запись.</span><span class="sxs-lookup"><span data-stu-id="00d7f-106">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="00d7f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="00d7f-107">Properties</span></span>

| <span data-ttu-id="00d7f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="00d7f-108">Property</span></span>     | <span data-ttu-id="00d7f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="00d7f-109">Type</span></span>        | <span data-ttu-id="00d7f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="00d7f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="00d7f-111">fieldId</span><span class="sxs-lookup"><span data-stu-id="00d7f-111">fieldId</span></span>|<span data-ttu-id="00d7f-112">String</span><span class="sxs-lookup"><span data-stu-id="00d7f-112">String</span></span>|<span data-ttu-id="00d7f-113">Имя поля для этих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="00d7f-113">The name of the field for this credential.</span></span> <span data-ttu-id="00d7f-114">Например, имя пользователя или пароль или phoneNumber.</span><span class="sxs-lookup"><span data-stu-id="00d7f-114">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="00d7f-115">Это определяется приложением.</span><span class="sxs-lookup"><span data-stu-id="00d7f-115">This is defined by the application.</span></span> <span data-ttu-id="00d7f-116">Должно отличаться от того, что указано в поле HTML в объекте Синглесигнонсеттингс/Password.</span><span class="sxs-lookup"><span data-stu-id="00d7f-116">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="00d7f-117">type</span><span class="sxs-lookup"><span data-stu-id="00d7f-117">type</span></span>|<span data-ttu-id="00d7f-118">String</span><span class="sxs-lookup"><span data-stu-id="00d7f-118">String</span></span>|<span data-ttu-id="00d7f-119">Тип для этих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="00d7f-119">The type for this credential.</span></span> <span data-ttu-id="00d7f-120">Допустимые значения: username, Password или other.</span><span class="sxs-lookup"><span data-stu-id="00d7f-120">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="00d7f-121">value</span><span class="sxs-lookup"><span data-stu-id="00d7f-121">value</span></span>|<span data-ttu-id="00d7f-122">String</span><span class="sxs-lookup"><span data-stu-id="00d7f-122">String</span></span>|<span data-ttu-id="00d7f-123">Значение для этих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="00d7f-123">The value for this credential.</span></span> <span data-ttu-id="00d7f-124">Например, мисуперхидденпассворд.</span><span class="sxs-lookup"><span data-stu-id="00d7f-124">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="00d7f-125">Примечание. значение для паролей доступно только для записи, его значение не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="00d7f-125">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00d7f-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00d7f-126">JSON representation</span></span>

<span data-ttu-id="00d7f-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00d7f-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credential",
  "baseType": null
}-->

```json
{
  "fieldId": "param_username",
  "value": "myusername",
  "type": "username"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


