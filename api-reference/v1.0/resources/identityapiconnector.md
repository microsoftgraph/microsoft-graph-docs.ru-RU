---
title: тип ресурса identityApiConnector
description: Представляет соединители API в клиенте Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8fc0ff1915bd76a35d9eb0c0041e1628fde41981
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883055"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="95f8c-103">тип ресурса identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="95f8c-103">identityApiConnector resource type</span></span>

<span data-ttu-id="95f8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95f8c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95f8c-105">Представляет соединители API в клиентах Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="95f8c-105">Represents API connectors in an Azure Active Directory (Azure AD) tenants.</span></span>

<span data-ttu-id="95f8c-106">Соединитель API, используемый в потоках пользователей самообслуживаемой регистрации Azure AD External Identities, позволяет вызывать API во время выполнения потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="95f8c-106">An API connector used in your Azure AD External Identities self-service sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="95f8c-107">Соединителя API предоставляет сведения, необходимые для вызова API, включая URL-адрес конечной точки и проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="95f8c-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="95f8c-108">Соединители API можно использовать на определенном шаге в потоке пользователей, чтобы повлиять на выполнение потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="95f8c-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="95f8c-109">Например, ответ API может заблокировать регистрацию пользователя, показать ошибку проверки ввода или переписать собранные атрибуты пользователя.</span><span class="sxs-lookup"><span data-stu-id="95f8c-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="95f8c-110">Используйте [API b2xIdentityUserFlow](b2xidentityuserflow.md) для использования соединителю API из потока пользователей самообслуживания внешних удостоверений.</span><span class="sxs-lookup"><span data-stu-id="95f8c-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="95f8c-111">Методы</span><span class="sxs-lookup"><span data-stu-id="95f8c-111">Methods</span></span>

|<span data-ttu-id="95f8c-112">Метод</span><span class="sxs-lookup"><span data-stu-id="95f8c-112">Method</span></span>|<span data-ttu-id="95f8c-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="95f8c-113">Return type</span></span>|<span data-ttu-id="95f8c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="95f8c-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95f8c-115">Список</span><span class="sxs-lookup"><span data-stu-id="95f8c-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="95f8c-116">[коллекция identityApiConnector](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="95f8c-116">[identityApiConnector](../resources/identityapiconnector.md) collection</span></span>| <span data-ttu-id="95f8c-117">Получить список соединителов API</span><span class="sxs-lookup"><span data-stu-id="95f8c-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="95f8c-118">Create</span><span class="sxs-lookup"><span data-stu-id="95f8c-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="95f8c-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="95f8c-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="95f8c-120">Создание нового соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="95f8c-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="95f8c-121">Get</span><span class="sxs-lookup"><span data-stu-id="95f8c-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="95f8c-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="95f8c-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="95f8c-123">Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="95f8c-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="95f8c-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="95f8c-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="95f8c-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="95f8c-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="95f8c-126">Обновление свойств соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="95f8c-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="95f8c-127">Загрузка клиентского сертификата</span><span class="sxs-lookup"><span data-stu-id="95f8c-127">Upload client certificate</span></span>](../api/identityapiconnector-uploadclientcertificate.md)|[<span data-ttu-id="95f8c-128">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="95f8c-128">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="95f8c-129">Загрузите клиентский сертификат для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="95f8c-129">Upload a client certificate to use for authentication.</span></span>|
|[<span data-ttu-id="95f8c-130">Delete</span><span class="sxs-lookup"><span data-stu-id="95f8c-130">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="95f8c-131">Нет</span><span class="sxs-lookup"><span data-stu-id="95f8c-131">None</span></span>|<span data-ttu-id="95f8c-132">Удаление соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="95f8c-132">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="95f8c-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="95f8c-133">Properties</span></span>

|<span data-ttu-id="95f8c-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="95f8c-134">Property</span></span>|<span data-ttu-id="95f8c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="95f8c-135">Type</span></span>|<span data-ttu-id="95f8c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="95f8c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95f8c-137">id</span><span class="sxs-lookup"><span data-stu-id="95f8c-137">id</span></span>|<span data-ttu-id="95f8c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="95f8c-138">String</span></span>|<span data-ttu-id="95f8c-139">Случайно созданный идентификатор соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="95f8c-139">The randomly generated identifier of the API connector.</span></span> |
|<span data-ttu-id="95f8c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="95f8c-140">displayName</span></span>|<span data-ttu-id="95f8c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="95f8c-141">String</span></span>| <span data-ttu-id="95f8c-142">Имя соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="95f8c-142">The name of the API connector.</span></span> |
|<span data-ttu-id="95f8c-143">targetUrl</span><span class="sxs-lookup"><span data-stu-id="95f8c-143">targetUrl</span></span>|<span data-ttu-id="95f8c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="95f8c-144">String</span></span>| <span data-ttu-id="95f8c-145">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="95f8c-145">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="95f8c-146">проверка подлинностиКонфигурация</span><span class="sxs-lookup"><span data-stu-id="95f8c-146">authenticationConfiguration</span></span>|[<span data-ttu-id="95f8c-147">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="95f8c-147">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="95f8c-148">Объект, описывая сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="95f8c-148">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="95f8c-149">Поддерживается клиентский сертификат Basic и PKCS 12.</span><span class="sxs-lookup"><span data-stu-id="95f8c-149">Basic and PKCS 12 client certificate are supported.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95f8c-150">Связи</span><span class="sxs-lookup"><span data-stu-id="95f8c-150">Relationships</span></span>

<span data-ttu-id="95f8c-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="95f8c-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95f8c-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95f8c-152">JSON representation</span></span>

<span data-ttu-id="95f8c-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95f8c-153">The following is a JSON representation of the resource.</span></span>
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
