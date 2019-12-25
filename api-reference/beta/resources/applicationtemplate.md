---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c34c083a4cfee63db724228d9390c7452ca5a92
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870948"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="d2cbe-103">Тип ресурса Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="d2cbe-103">applicationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2cbe-104">Представляет приложение в [коллекции приложений Azure AD](/azure/active-directory/saas-apps/tutorial-list).</span><span class="sxs-lookup"><span data-stu-id="d2cbe-104">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="d2cbe-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d2cbe-105">Methods</span></span>

| <span data-ttu-id="d2cbe-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d2cbe-106">Method</span></span>       | <span data-ttu-id="d2cbe-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d2cbe-107">Return Type</span></span> | <span data-ttu-id="d2cbe-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d2cbe-108">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="d2cbe-109">Список Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="d2cbe-109">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="d2cbe-110">аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="d2cbe-110">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="d2cbe-111">Получение списка объектов Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-111">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="d2cbe-112">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="d2cbe-112">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="d2cbe-113">аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="d2cbe-113">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="d2cbe-114">Чтение свойств и связей объекта Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-114">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="d2cbe-115">Создание экземпляра Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="d2cbe-115">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="d2cbe-116">аппликатионсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="d2cbe-116">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="d2cbe-117">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-117">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="d2cbe-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2cbe-118">Properties</span></span>

| <span data-ttu-id="d2cbe-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2cbe-119">Property</span></span>     | <span data-ttu-id="d2cbe-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d2cbe-120">Type</span></span>        | <span data-ttu-id="d2cbe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d2cbe-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2cbe-122">categories</span><span class="sxs-lookup"><span data-stu-id="d2cbe-122">categories</span></span>|<span data-ttu-id="d2cbe-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d2cbe-123">String collection</span></span>|<span data-ttu-id="d2cbe-124">Список категорий для приложения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-124">The list of categories for the application.</span></span> <span data-ttu-id="d2cbe-125">Поддерживаются следующие значения: `Collaboration`, `Business Management`, `Consumer`,`Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Web design & hosting`,,,,,,,,, `Tools, Travel`, `Telecommunications`,,,,,,,,,,,,,, и. `Project management` `ERP` `Finance`</span><span class="sxs-lookup"><span data-stu-id="d2cbe-125">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="d2cbe-126">description</span><span class="sxs-lookup"><span data-stu-id="d2cbe-126">description</span></span>|<span data-ttu-id="d2cbe-127">String</span><span class="sxs-lookup"><span data-stu-id="d2cbe-127">String</span></span>|<span data-ttu-id="d2cbe-128">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-128">A description of the application.</span></span>|
|<span data-ttu-id="d2cbe-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d2cbe-129">displayName</span></span>|<span data-ttu-id="d2cbe-130">Строка</span><span class="sxs-lookup"><span data-stu-id="d2cbe-130">String</span></span>|<span data-ttu-id="d2cbe-131">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-131">The name of the application.</span></span>|
|<span data-ttu-id="d2cbe-132">хомепажеурл</span><span class="sxs-lookup"><span data-stu-id="d2cbe-132">homePageUrl</span></span>|<span data-ttu-id="d2cbe-133">String</span><span class="sxs-lookup"><span data-stu-id="d2cbe-133">String</span></span>|<span data-ttu-id="d2cbe-134">URL-адрес домашней страницы приложения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-134">The home page URL of the application.</span></span>|
|<span data-ttu-id="d2cbe-135">id</span><span class="sxs-lookup"><span data-stu-id="d2cbe-135">id</span></span>|<span data-ttu-id="d2cbe-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d2cbe-136">String</span></span>| <span data-ttu-id="d2cbe-137">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-137">Unique identifier for the application.</span></span> <span data-ttu-id="d2cbe-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-138">Read-only.</span></span>|
|<span data-ttu-id="d2cbe-139">logoUrl</span><span class="sxs-lookup"><span data-stu-id="d2cbe-139">logoUrl</span></span>|<span data-ttu-id="d2cbe-140">String</span><span class="sxs-lookup"><span data-stu-id="d2cbe-140">String</span></span>|<span data-ttu-id="d2cbe-141">URL-адрес для получения логотипа для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-141">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="d2cbe-142">publisher</span><span class="sxs-lookup"><span data-stu-id="d2cbe-142">publisher</span></span>|<span data-ttu-id="d2cbe-143">String</span><span class="sxs-lookup"><span data-stu-id="d2cbe-143">String</span></span>|<span data-ttu-id="d2cbe-144">Имя издателя для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-144">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="d2cbe-145">суппортедпровисионингтипес</span><span class="sxs-lookup"><span data-stu-id="d2cbe-145">supportedProvisioningTypes</span></span>|<span data-ttu-id="d2cbe-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d2cbe-146">String collection</span></span>|<span data-ttu-id="d2cbe-147">Список режимов подготовки, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-147">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="d2cbe-148">Единственное допустимое значение: `sync`.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-148">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="d2cbe-149">суппортедсинглесигнонмодес</span><span class="sxs-lookup"><span data-stu-id="d2cbe-149">supportedSingleSignOnModes</span></span>|<span data-ttu-id="d2cbe-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d2cbe-150">String collection</span></span>|<span data-ttu-id="d2cbe-151">Список режимов единого входа, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-151">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="d2cbe-152">`password`Поддерживаемые значения: `saml`, `external`, и. `oidc`</span><span class="sxs-lookup"><span data-stu-id="d2cbe-152">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2cbe-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="d2cbe-153">Relationships</span></span>

<span data-ttu-id="d2cbe-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2cbe-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d2cbe-155">JSON representation</span></span>

<span data-ttu-id="d2cbe-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2cbe-156">The following is a JSON representation of the resource.</span></span>

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
