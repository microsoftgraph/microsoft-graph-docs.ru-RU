---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a8e1f4cb365f86df32e32ed568aa3a96d1c090f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147937"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="a29cb-103">Тип ресурса Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a29cb-103">applicationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a29cb-104">Представляет приложение в [коллекции приложений Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list).</span><span class="sxs-lookup"><span data-stu-id="a29cb-104">Represents an application in the [Azure AD application gallery](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="a29cb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a29cb-105">Methods</span></span>

| <span data-ttu-id="a29cb-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a29cb-106">Method</span></span>       | <span data-ttu-id="a29cb-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a29cb-107">Return Type</span></span> | <span data-ttu-id="a29cb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a29cb-108">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="a29cb-109">Список Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a29cb-109">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="a29cb-110">Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a29cb-110">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="a29cb-111">Получение списка объектов Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="a29cb-111">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="a29cb-112">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a29cb-112">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="a29cb-113">Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a29cb-113">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="a29cb-114">Чтение свойств и связей объекта Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="a29cb-114">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="a29cb-115">Создание экземпляра Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a29cb-115">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="a29cb-116">АппликатионсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="a29cb-116">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="a29cb-117">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="a29cb-117">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="a29cb-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a29cb-118">Properties</span></span>

| <span data-ttu-id="a29cb-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a29cb-119">Property</span></span>     | <span data-ttu-id="a29cb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a29cb-120">Type</span></span>        | <span data-ttu-id="a29cb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a29cb-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a29cb-122">categories</span><span class="sxs-lookup"><span data-stu-id="a29cb-122">categories</span></span>|<span data-ttu-id="a29cb-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a29cb-123">String collection</span></span>|<span data-ttu-id="a29cb-124">Список категорий для приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-124">The list of categories for the application.</span></span> <span data-ttu-id="a29cb-125">Допустимые `Collaboration`значения:, `Business Management`, `Consumer`,`Content management` `CRM` `Data services` `Developer services` `E-commerce` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Human resources` `Finance` `Health`,,,,,,,,,,,,,,,,,,,, `Education` `ERP` , `Project management`, `Telecommunications`, `Tools, Travel`, и `Web design & hosting`.</span><span class="sxs-lookup"><span data-stu-id="a29cb-125">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="a29cb-126">description</span><span class="sxs-lookup"><span data-stu-id="a29cb-126">description</span></span>|<span data-ttu-id="a29cb-127">String</span><span class="sxs-lookup"><span data-stu-id="a29cb-127">String</span></span>|<span data-ttu-id="a29cb-128">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-128">A description of the application.</span></span>|
|<span data-ttu-id="a29cb-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a29cb-129">displayName</span></span>|<span data-ttu-id="a29cb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a29cb-130">String</span></span>|<span data-ttu-id="a29cb-131">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-131">The name of the application.</span></span>|
|<span data-ttu-id="a29cb-132">Хомепажеурл</span><span class="sxs-lookup"><span data-stu-id="a29cb-132">homePageUrl</span></span>|<span data-ttu-id="a29cb-133">String</span><span class="sxs-lookup"><span data-stu-id="a29cb-133">String</span></span>|<span data-ttu-id="a29cb-134">URL-адрес домашней страницы приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-134">The home page URL of the application.</span></span>|
|<span data-ttu-id="a29cb-135">id</span><span class="sxs-lookup"><span data-stu-id="a29cb-135">id</span></span>|<span data-ttu-id="a29cb-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a29cb-136">String</span></span>| <span data-ttu-id="a29cb-137">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-137">Unique identifier for the application.</span></span> <span data-ttu-id="a29cb-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-138">Read-only.</span></span>|
|<span data-ttu-id="a29cb-139">logoUrl</span><span class="sxs-lookup"><span data-stu-id="a29cb-139">logoUrl</span></span>|<span data-ttu-id="a29cb-140">String</span><span class="sxs-lookup"><span data-stu-id="a29cb-140">String</span></span>|<span data-ttu-id="a29cb-141">URL-адрес для получения логотипа для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-141">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="a29cb-142">publisher</span><span class="sxs-lookup"><span data-stu-id="a29cb-142">publisher</span></span>|<span data-ttu-id="a29cb-143">String</span><span class="sxs-lookup"><span data-stu-id="a29cb-143">String</span></span>|<span data-ttu-id="a29cb-144">Имя издателя для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cb-144">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="a29cb-145">Суппортедпровисионингтипес</span><span class="sxs-lookup"><span data-stu-id="a29cb-145">supportedProvisioningTypes</span></span>|<span data-ttu-id="a29cb-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a29cb-146">String collection</span></span>|<span data-ttu-id="a29cb-147">Список режимов подготовки, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a29cb-147">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="a29cb-148">Единственное допустимое значение: `sync`.</span><span class="sxs-lookup"><span data-stu-id="a29cb-148">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="a29cb-149">Суппортедсинглесигнонмодес</span><span class="sxs-lookup"><span data-stu-id="a29cb-149">supportedSingleSignOnModes</span></span>|<span data-ttu-id="a29cb-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a29cb-150">String collection</span></span>|<span data-ttu-id="a29cb-151">Список режимов единого входа, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a29cb-151">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="a29cb-152">`password`Поддерживаемые значения: `saml`, `external`, и. `oidc`</span><span class="sxs-lookup"><span data-stu-id="a29cb-152">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a29cb-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="a29cb-153">Relationships</span></span>

<span data-ttu-id="a29cb-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a29cb-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a29cb-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a29cb-155">JSON representation</span></span>

<span data-ttu-id="a29cb-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a29cb-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
