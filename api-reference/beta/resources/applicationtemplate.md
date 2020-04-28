---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c707a9010103f4226e62782a83891ff880a245e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508263"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="cf99f-103">Тип ресурса Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="cf99f-103">applicationTemplate resource type</span></span>

<span data-ttu-id="cf99f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf99f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf99f-105">Представляет приложение в [коллекции приложений Azure AD](/azure/active-directory/saas-apps/tutorial-list).</span><span class="sxs-lookup"><span data-stu-id="cf99f-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="cf99f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cf99f-106">Methods</span></span>

| <span data-ttu-id="cf99f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cf99f-107">Method</span></span>       | <span data-ttu-id="cf99f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cf99f-108">Return Type</span></span> | <span data-ttu-id="cf99f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cf99f-109">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="cf99f-110">Список Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="cf99f-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="cf99f-111">аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="cf99f-111">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="cf99f-112">Получение списка объектов Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="cf99f-112">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="cf99f-113">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="cf99f-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="cf99f-114">аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="cf99f-114">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="cf99f-115">Чтение свойств и связей объекта Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="cf99f-115">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="cf99f-116">Создание экземпляра Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="cf99f-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="cf99f-117">аппликатионсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="cf99f-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="cf99f-118">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="cf99f-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="cf99f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf99f-119">Properties</span></span>

| <span data-ttu-id="cf99f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf99f-120">Property</span></span>     | <span data-ttu-id="cf99f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cf99f-121">Type</span></span>        | <span data-ttu-id="cf99f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cf99f-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf99f-123">categories</span><span class="sxs-lookup"><span data-stu-id="cf99f-123">categories</span></span>|<span data-ttu-id="cf99f-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf99f-124">String collection</span></span>|<span data-ttu-id="cf99f-125">Список категорий для приложения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-125">The list of categories for the application.</span></span> <span data-ttu-id="cf99f-126">Поддерживаются следующие значения: `Collaboration`, `Business Management`, `Consumer`,`Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Web design & hosting`,,,,,,,,, `Tools, Travel`, `Telecommunications`,,,,,,,,,,,,,, и. `Project management` `ERP` `Finance`</span><span class="sxs-lookup"><span data-stu-id="cf99f-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="cf99f-127">description</span><span class="sxs-lookup"><span data-stu-id="cf99f-127">description</span></span>|<span data-ttu-id="cf99f-128">String</span><span class="sxs-lookup"><span data-stu-id="cf99f-128">String</span></span>|<span data-ttu-id="cf99f-129">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-129">A description of the application.</span></span>|
|<span data-ttu-id="cf99f-130">displayName</span><span class="sxs-lookup"><span data-stu-id="cf99f-130">displayName</span></span>|<span data-ttu-id="cf99f-131">Строка</span><span class="sxs-lookup"><span data-stu-id="cf99f-131">String</span></span>|<span data-ttu-id="cf99f-132">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-132">The name of the application.</span></span>|
|<span data-ttu-id="cf99f-133">хомепажеурл</span><span class="sxs-lookup"><span data-stu-id="cf99f-133">homePageUrl</span></span>|<span data-ttu-id="cf99f-134">String</span><span class="sxs-lookup"><span data-stu-id="cf99f-134">String</span></span>|<span data-ttu-id="cf99f-135">URL-адрес домашней страницы приложения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-135">The home page URL of the application.</span></span>|
|<span data-ttu-id="cf99f-136">id</span><span class="sxs-lookup"><span data-stu-id="cf99f-136">id</span></span>|<span data-ttu-id="cf99f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cf99f-137">String</span></span>| <span data-ttu-id="cf99f-138">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-138">Unique identifier for the application.</span></span> <span data-ttu-id="cf99f-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-139">Read-only.</span></span>|
|<span data-ttu-id="cf99f-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="cf99f-140">logoUrl</span></span>|<span data-ttu-id="cf99f-141">String</span><span class="sxs-lookup"><span data-stu-id="cf99f-141">String</span></span>|<span data-ttu-id="cf99f-142">URL-адрес для получения логотипа для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-142">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="cf99f-143">publisher</span><span class="sxs-lookup"><span data-stu-id="cf99f-143">publisher</span></span>|<span data-ttu-id="cf99f-144">String</span><span class="sxs-lookup"><span data-stu-id="cf99f-144">String</span></span>|<span data-ttu-id="cf99f-145">Имя издателя для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="cf99f-145">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="cf99f-146">суппортедпровисионингтипес</span><span class="sxs-lookup"><span data-stu-id="cf99f-146">supportedProvisioningTypes</span></span>|<span data-ttu-id="cf99f-147">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="cf99f-147">String collection</span></span>|<span data-ttu-id="cf99f-148">Список режимов подготовки, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cf99f-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="cf99f-149">Единственное допустимое значение: `sync`.</span><span class="sxs-lookup"><span data-stu-id="cf99f-149">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="cf99f-150">суппортедсинглесигнонмодес</span><span class="sxs-lookup"><span data-stu-id="cf99f-150">supportedSingleSignOnModes</span></span>|<span data-ttu-id="cf99f-151">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="cf99f-151">String collection</span></span>|<span data-ttu-id="cf99f-152">Список режимов единого входа, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cf99f-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="cf99f-153">`password`Поддерживаемые значения: `saml`, `external`, и. `oidc`</span><span class="sxs-lookup"><span data-stu-id="cf99f-153">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf99f-154">Связи</span><span class="sxs-lookup"><span data-stu-id="cf99f-154">Relationships</span></span>

<span data-ttu-id="cf99f-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cf99f-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf99f-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cf99f-156">JSON representation</span></span>

<span data-ttu-id="cf99f-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf99f-157">The following is a JSON representation of the resource.</span></span>

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
