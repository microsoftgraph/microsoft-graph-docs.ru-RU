---
title: Тип ресурса Усераккаунтинформатион
description: Тип ресурса Усераккаунтинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0bdb0bd3856e8eaf55d19d01a8566a34810051c7
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949491"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="239b7-103">Тип ресурса Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="239b7-103">userAccountInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="239b7-104">Представляет сведения, специально связанные с учетной записью пользователя, будь то учетная запись Azure AD или учетная запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="239b7-104">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="239b7-105">Идентификатор сущности задается соответствующим идентификаторам Azure AD AD или CID учетной записи Майкрософт соответственно.</span><span class="sxs-lookup"><span data-stu-id="239b7-105">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="239b7-106">Эти поля доступны только для чтения через Microsoft Graph и должны редактироваться с помощью профиля пользователя или администратора клиента для соответствующего интерфейса.</span><span class="sxs-lookup"><span data-stu-id="239b7-106">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="239b7-107">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="239b7-107">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="239b7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="239b7-108">Methods</span></span>

| <span data-ttu-id="239b7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="239b7-109">Method</span></span>                                                             | <span data-ttu-id="239b7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="239b7-110">Return Type</span></span>                                         | <span data-ttu-id="239b7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="239b7-111">Description</span></span>                                                         |
|:-------------------------------------------------------------------|:----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="239b7-112">Получение Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="239b7-112">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md) | [<span data-ttu-id="239b7-113">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="239b7-113">userAccountInformation</span></span>](useraccountinformation.md) | <span data-ttu-id="239b7-114">Чтение свойств и связей объекта **усераккаунтинформатион** .</span><span class="sxs-lookup"><span data-stu-id="239b7-114">Read the properties and relationships of a **userAccountInformation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="239b7-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="239b7-115">Properties</span></span>

| <span data-ttu-id="239b7-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="239b7-116">Property</span></span>            | <span data-ttu-id="239b7-117">Тип</span><span class="sxs-lookup"><span data-stu-id="239b7-117">Type</span></span>                       | <span data-ttu-id="239b7-118">Описание</span><span class="sxs-lookup"><span data-stu-id="239b7-118">Description</span></span>                                                                                                                              |
|:--------------------|:---------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="239b7-119">ageGroup</span><span class="sxs-lookup"><span data-stu-id="239b7-119">ageGroup</span></span>             |<span data-ttu-id="239b7-120">String</span><span class="sxs-lookup"><span data-stu-id="239b7-120">String</span></span>                      | <span data-ttu-id="239b7-121">Показывает группу возрастных пользователей.</span><span class="sxs-lookup"><span data-stu-id="239b7-121">Shows the age group of user.</span></span> <span data-ttu-id="239b7-122">Допустимые `null`значения `minor`, `notAdult` и `adult` они создаются каталогом и не могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="239b7-122">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="239b7-123">countryCode</span><span class="sxs-lookup"><span data-stu-id="239b7-123">countryCode</span></span>          |<span data-ttu-id="239b7-124">String</span><span class="sxs-lookup"><span data-stu-id="239b7-124">String</span></span>|                     | <span data-ttu-id="239b7-125">Содержит двухбуквенный код страны, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="239b7-125">Contains the two-character country code associated with the users account.</span></span>                                                                |
|<span data-ttu-id="239b7-126">преферредлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="239b7-126">preferredLanguageTag</span></span> |[<span data-ttu-id="239b7-127">localeInfo</span><span class="sxs-lookup"><span data-stu-id="239b7-127">localeInfo</span></span>](localeinfo.md) | <span data-ttu-id="239b7-128">Содержит язык, который пользователь связал с учетной записью как предпочитаемый.</span><span class="sxs-lookup"><span data-stu-id="239b7-128">Contains the language the user has associated as preferred for the account.</span></span>                                                              |
|<span data-ttu-id="239b7-129">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="239b7-129">userPrincipalName</span></span>    |<span data-ttu-id="239b7-130">String</span><span class="sxs-lookup"><span data-stu-id="239b7-130">String</span></span>                      | <span data-ttu-id="239b7-131">Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="239b7-131">The user principal name (UPN) of the user associated with the account.</span></span>                                                                   |

## <a name="relationships"></a><span data-ttu-id="239b7-132">Связи</span><span class="sxs-lookup"><span data-stu-id="239b7-132">Relationships</span></span>

<span data-ttu-id="239b7-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="239b7-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="239b7-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="239b7-134">JSON representation</span></span>

<span data-ttu-id="239b7-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="239b7-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": ""
}-->

```json
{
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {"@odata.type": "microsoft.graph.localeInfo"},
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAccountInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
