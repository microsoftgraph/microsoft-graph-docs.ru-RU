---
title: Тип ресурса appleManagedIdentityProvider
description: Представляет поставщика удостоверений Apple в клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ee02900b6d41695d49d7c5ee38d834c676f69603
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491194"
---
# <a name="applemanagedidentityprovider-resource-type"></a><span data-ttu-id="2c36d-103">Тип ресурса appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="2c36d-103">appleManagedIdentityProvider resource type</span></span>
<span data-ttu-id="2c36d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c36d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c36d-105">Вы можете настроить Apple в качестве поставщика удостоверений социальных сетей для клиента Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="2c36d-105">You can configure Apple as a social identity provider for an Azure AD B2C tenant.</span></span> <span data-ttu-id="2c36d-106">На основе информации, которую предоставляет Apple, API создает секрет клиента.</span><span class="sxs-lookup"><span data-stu-id="2c36d-106">Based on the information Apple provides, the API will generate a client secret.</span></span> <span data-ttu-id="2c36d-107">Apple нужно, чтобы секрет обновлялся каждые шесть месяцев.</span><span class="sxs-lookup"><span data-stu-id="2c36d-107">Apple needs the secret to be renewed every six months.</span></span> <span data-ttu-id="2c36d-108">Потребуется изменять секрет вручную.</span><span class="sxs-lookup"><span data-stu-id="2c36d-108">You will have to maunally rotate the secret.</span></span>

<span data-ttu-id="2c36d-109">Этот тип наследуется от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="2c36d-109">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2c36d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="2c36d-110">Methods</span></span>

| <span data-ttu-id="2c36d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="2c36d-111">Method</span></span>       | <span data-ttu-id="2c36d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2c36d-112">Return Type</span></span>  |<span data-ttu-id="2c36d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="2c36d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c36d-114">Список</span><span class="sxs-lookup"><span data-stu-id="2c36d-114">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="2c36d-115">Коллекция identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="2c36d-115">identityProviderBase collection</span></span>|<span data-ttu-id="2c36d-116">Получение всех поставщиков удостоверений, настроенных в клиенте, включая поставщиков удостоверений Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-116">Retrieve all identity providers configured in a tenant including the Apple identity providers.</span></span>|
|[<span data-ttu-id="2c36d-117">Создание</span><span class="sxs-lookup"><span data-stu-id="2c36d-117">Create</span></span>](../api/identityproviderbase-post-identityproviders.md)|<span data-ttu-id="2c36d-118">appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="2c36d-118">appleManagedIdentityProvider</span></span> |<span data-ttu-id="2c36d-119">Создание конфигурации поставщика удостоверений Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-119">Create a new Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="2c36d-120">Получение</span><span class="sxs-lookup"><span data-stu-id="2c36d-120">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="2c36d-121">appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="2c36d-121">appleManagedIdentityProvider</span></span> |<span data-ttu-id="2c36d-122">Получение свойств конфигурации поставщика удостоверений Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-122">Retrieve properties of the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="2c36d-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="2c36d-123">Update</span></span>](../api/identityproviderbase-update.md)|<span data-ttu-id="2c36d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="2c36d-124">None</span></span>|<span data-ttu-id="2c36d-125">Обновление конфигурации поставщика удостоверений Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-125">Update the Apple identity provider configuration.</span></span>|
|<span data-ttu-id="2c36d-126">[удаление](../api/identityproviderbase-delete.md);</span><span class="sxs-lookup"><span data-stu-id="2c36d-126">[Delete](../api/identityproviderbase-delete.md)</span></span>|<span data-ttu-id="2c36d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2c36d-127">None</span></span>|<span data-ttu-id="2c36d-128">Удаление конфигурации поставщика удостоверений Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-128">Delete the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="2c36d-129">Перечисление доступных типов поставщиков</span><span class="sxs-lookup"><span data-stu-id="2c36d-129">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="2c36d-130">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2c36d-130">String collection</span></span>|<span data-ttu-id="2c36d-131">Получение всех типов поставщиков удостоверений, доступных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2c36d-131">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c36d-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c36d-132">Properties</span></span>

|<span data-ttu-id="2c36d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c36d-133">Property</span></span>|<span data-ttu-id="2c36d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="2c36d-134">Type</span></span>|<span data-ttu-id="2c36d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="2c36d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c36d-136">developerId</span><span class="sxs-lookup"><span data-stu-id="2c36d-136">developerId</span></span>|<span data-ttu-id="2c36d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2c36d-137">String</span></span>|<span data-ttu-id="2c36d-138">Идентификатор разработчика Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-138">The Apple developer identifier.</span></span> <span data-ttu-id="2c36d-139">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2c36d-139">Required.</span></span>|
|<span data-ttu-id="2c36d-140">serviceId</span><span class="sxs-lookup"><span data-stu-id="2c36d-140">serviceId</span></span>|<span data-ttu-id="2c36d-141">Строка</span><span class="sxs-lookup"><span data-stu-id="2c36d-141">String</span></span>|<span data-ttu-id="2c36d-142">Идентификатор службы Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-142">The Apple service identifier.</span></span> <span data-ttu-id="2c36d-143">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2c36d-143">Required.</span></span>|
|<span data-ttu-id="2c36d-144">keyId</span><span class="sxs-lookup"><span data-stu-id="2c36d-144">keyId</span></span>|<span data-ttu-id="2c36d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="2c36d-145">String</span></span>|<span data-ttu-id="2c36d-146">Идентификатор ключа Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-146">The Apple key identifier.</span></span> <span data-ttu-id="2c36d-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2c36d-147">Required.</span></span>|
|<span data-ttu-id="2c36d-148">certificateData</span><span class="sxs-lookup"><span data-stu-id="2c36d-148">certificateData</span></span>|<span data-ttu-id="2c36d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="2c36d-149">String</span></span>|<span data-ttu-id="2c36d-150">Данные сертификата, являющиеся длинной строкой текста из сертификата. Могут иметь значение NULL.</span><span class="sxs-lookup"><span data-stu-id="2c36d-150">The certificate data which is a long string of text from the certificate, can be null.</span></span>|
|<span data-ttu-id="2c36d-151">id</span><span class="sxs-lookup"><span data-stu-id="2c36d-151">id</span></span>|<span data-ttu-id="2c36d-152">String</span><span class="sxs-lookup"><span data-stu-id="2c36d-152">String</span></span>|<span data-ttu-id="2c36d-153">Идентификатор поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2c36d-153">The identifier of the identity provider.</span></span> <span data-ttu-id="2c36d-154">Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="2c36d-154">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="2c36d-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c36d-155">Read-only.</span></span>|
|<span data-ttu-id="2c36d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="2c36d-156">displayName</span></span>|<span data-ttu-id="2c36d-157">String</span><span class="sxs-lookup"><span data-stu-id="2c36d-157">String</span></span>|<span data-ttu-id="2c36d-158">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2c36d-158">The display name of the identity provider.</span></span> <span data-ttu-id="2c36d-159">Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="2c36d-159">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|

<span data-ttu-id="2c36d-160">Вы можете найти developerId, serviceId, keyId и certificateData на портале разработчика Apple.</span><span class="sxs-lookup"><span data-stu-id="2c36d-160">You can find the developerId, serviceId, keyId and the certificateData from the Apple developer portal.</span></span> <span data-ttu-id="2c36d-161">Дополнительные сведения см. в руководстве по [созданию приложения Apple ID](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)</span><span class="sxs-lookup"><span data-stu-id="2c36d-161">For nore details you can follow the guide to [create an Apple ID application](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c36d-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c36d-162">JSON representation</span></span>

<span data-ttu-id="2c36d-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c36d-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```json
{
    "id": "String",
    "displayName": "String",
    "developerId": "String",
    "serviceId": "String",
    "keyId": "String",
    "certificateData": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "appleIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
