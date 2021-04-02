---
title: тип ресурса identityApiConnector
description: Представляет соединители API в клиенте Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7ecb96a9ca2f4397c1f0ee52908a7802374df0f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508108"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="97e09-103">тип ресурса identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="97e09-103">identityApiConnector resource type</span></span>

<span data-ttu-id="97e09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97e09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97e09-105">Представляет соединители API в клиентах Azure Active Directory (Azure AD) и Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="97e09-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="97e09-106">Соединитель API, используемый в вашей самообслуживке Azure AD External Identities и потоках пользователей для регистрации Azure AD B2C, позволяет вызывать API во время выполнения потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="97e09-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="97e09-107">Соединителя API предоставляет сведения, необходимые для вызова API, включая URL-адрес конечной точки и проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="97e09-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="97e09-108">Соединители API можно использовать на определенном шаге в потоке пользователей, чтобы повлиять на выполнение потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="97e09-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="97e09-109">Например, ответ API может заблокировать регистрацию пользователя, показать ошибку проверки ввода или переписать собранные атрибуты пользователя.</span><span class="sxs-lookup"><span data-stu-id="97e09-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="97e09-110">Используйте [API b2xIdentityUserFlow](b2xidentityuserflow.md) для использования соединителю API из потока пользователей самообслуживания внешних удостоверений.</span><span class="sxs-lookup"><span data-stu-id="97e09-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="97e09-111">Методы</span><span class="sxs-lookup"><span data-stu-id="97e09-111">Methods</span></span>

|<span data-ttu-id="97e09-112">Метод</span><span class="sxs-lookup"><span data-stu-id="97e09-112">Method</span></span>|<span data-ttu-id="97e09-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="97e09-113">Return type</span></span>|<span data-ttu-id="97e09-114">Описание</span><span class="sxs-lookup"><span data-stu-id="97e09-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97e09-115">Список</span><span class="sxs-lookup"><span data-stu-id="97e09-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="97e09-116">[коллекция identityApiConnector](identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="97e09-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="97e09-117">Получить список соединителов API</span><span class="sxs-lookup"><span data-stu-id="97e09-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="97e09-118">Создание</span><span class="sxs-lookup"><span data-stu-id="97e09-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="97e09-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="97e09-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="97e09-120">Создание нового соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="97e09-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="97e09-121">Получение</span><span class="sxs-lookup"><span data-stu-id="97e09-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="97e09-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="97e09-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="97e09-123">Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="97e09-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="97e09-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="97e09-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="97e09-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="97e09-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="97e09-126">Обновление свойств соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="97e09-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="97e09-127">Загрузка клиентского сертификата</span><span class="sxs-lookup"><span data-stu-id="97e09-127">Upload client certificate</span></span>](../api/identityapiconnector-uploadclientcertificate.md)|[<span data-ttu-id="97e09-128">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="97e09-128">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="97e09-129">Загрузите клиентский сертификат для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="97e09-129">Upload a client certificate to use for authentication.</span></span>|
|[<span data-ttu-id="97e09-130">Удаление</span><span class="sxs-lookup"><span data-stu-id="97e09-130">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="97e09-131">Нет</span><span class="sxs-lookup"><span data-stu-id="97e09-131">None</span></span>|<span data-ttu-id="97e09-132">Удаление соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="97e09-132">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="97e09-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="97e09-133">Properties</span></span>

|<span data-ttu-id="97e09-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="97e09-134">Property</span></span>|<span data-ttu-id="97e09-135">Тип</span><span class="sxs-lookup"><span data-stu-id="97e09-135">Type</span></span>|<span data-ttu-id="97e09-136">Описание</span><span class="sxs-lookup"><span data-stu-id="97e09-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97e09-137">id</span><span class="sxs-lookup"><span data-stu-id="97e09-137">id</span></span>|<span data-ttu-id="97e09-138">String</span><span class="sxs-lookup"><span data-stu-id="97e09-138">String</span></span>|<span data-ttu-id="97e09-139">Случайно созданный ID соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="97e09-139">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="97e09-140">displayName</span><span class="sxs-lookup"><span data-stu-id="97e09-140">displayName</span></span>|<span data-ttu-id="97e09-141">String</span><span class="sxs-lookup"><span data-stu-id="97e09-141">String</span></span>| <span data-ttu-id="97e09-142">Имя соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="97e09-142">The name of the API connector.</span></span> |
|<span data-ttu-id="97e09-143">targetUrl</span><span class="sxs-lookup"><span data-stu-id="97e09-143">targetUrl</span></span>|<span data-ttu-id="97e09-144">String</span><span class="sxs-lookup"><span data-stu-id="97e09-144">String</span></span>| <span data-ttu-id="97e09-145">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="97e09-145">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="97e09-146">проверка подлинностиКонфигурация</span><span class="sxs-lookup"><span data-stu-id="97e09-146">authenticationConfiguration</span></span>|[<span data-ttu-id="97e09-147">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="97e09-147">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="97e09-148">Объект, описывая сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="97e09-148">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="97e09-149">Поддерживается клиентский сертификат Basic и PKCS 12.</span><span class="sxs-lookup"><span data-stu-id="97e09-149">Basic and PKCS 12 client certificate are supported.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97e09-150">Связи</span><span class="sxs-lookup"><span data-stu-id="97e09-150">Relationships</span></span>

<span data-ttu-id="97e09-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97e09-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97e09-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97e09-152">JSON representation</span></span>

<span data-ttu-id="97e09-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97e09-153">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "targetUrl": "String",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  }
}
```
