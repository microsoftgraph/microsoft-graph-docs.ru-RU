---
title: Тип ресурса Credential
description: Указывает одну учетную запись, используемую для входа в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3b23249d7c0b898344113c5bcfe950c207891250
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658886"
---
# <a name="credential-resource-type"></a><span data-ttu-id="2f818-103">Тип ресурса Credential</span><span class="sxs-lookup"><span data-stu-id="2f818-103">credential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f818-104">Указывает одну учетную запись, используемую для входа в приложение.</span><span class="sxs-lookup"><span data-stu-id="2f818-104">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="2f818-105">Например, username это один учетный набор учетных данных, пароль — это еще одна учетная запись.</span><span class="sxs-lookup"><span data-stu-id="2f818-105">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="2f818-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f818-106">Properties</span></span>

| <span data-ttu-id="2f818-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f818-107">Property</span></span>     | <span data-ttu-id="2f818-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2f818-108">Type</span></span>        | <span data-ttu-id="2f818-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f818-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f818-110">fieldId</span><span class="sxs-lookup"><span data-stu-id="2f818-110">fieldId</span></span>|<span data-ttu-id="2f818-111">String</span><span class="sxs-lookup"><span data-stu-id="2f818-111">String</span></span>|<span data-ttu-id="2f818-112">Имя поля для этих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2f818-112">The name of the field for this credential.</span></span> <span data-ttu-id="2f818-113">Например, имя пользователя или пароль или phoneNumber.</span><span class="sxs-lookup"><span data-stu-id="2f818-113">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="2f818-114">Это определяется приложением.</span><span class="sxs-lookup"><span data-stu-id="2f818-114">This is defined by the application.</span></span> <span data-ttu-id="2f818-115">Должно отличаться от того, что указано в поле HTML в объекте Синглесигнонсеттингс/Password.</span><span class="sxs-lookup"><span data-stu-id="2f818-115">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="2f818-116">type</span><span class="sxs-lookup"><span data-stu-id="2f818-116">type</span></span>|<span data-ttu-id="2f818-117">String</span><span class="sxs-lookup"><span data-stu-id="2f818-117">String</span></span>|<span data-ttu-id="2f818-118">Тип для этих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2f818-118">The type for this credential.</span></span> <span data-ttu-id="2f818-119">Допустимые значения: username, Password или other.</span><span class="sxs-lookup"><span data-stu-id="2f818-119">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="2f818-120">value</span><span class="sxs-lookup"><span data-stu-id="2f818-120">value</span></span>|<span data-ttu-id="2f818-121">String</span><span class="sxs-lookup"><span data-stu-id="2f818-121">String</span></span>|<span data-ttu-id="2f818-122">Значение для этих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2f818-122">The value for this credential.</span></span> <span data-ttu-id="2f818-123">Например, мисуперхидденпассворд.</span><span class="sxs-lookup"><span data-stu-id="2f818-123">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="2f818-124">Примечание. значение для паролей доступно только для записи, его значение не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="2f818-124">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f818-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f818-125">JSON representation</span></span>

<span data-ttu-id="2f818-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f818-126">The following is a JSON representation of the resource.</span></span>

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
