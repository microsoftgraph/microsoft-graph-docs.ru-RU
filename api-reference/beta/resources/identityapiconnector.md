---
title: тип ресурса identityApiConnector
description: Представляет соединители API в клиенте Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a267fdb60dfcbcbbadfe75c65d49137f46425434
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443029"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="72684-103">тип ресурса identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="72684-103">identityApiConnector resource type</span></span>

<span data-ttu-id="72684-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72684-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72684-105">Представляет соединители API в клиентах Azure Active Directory (Azure AD) и Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="72684-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="72684-106">Соединитель API, используемый в вашей самообслуживке Azure AD External Identities и потоках пользователей для регистрации Azure AD B2C, позволяет вызывать API во время выполнения потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="72684-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="72684-107">Соединителя API предоставляет сведения, необходимые для вызова API, включая URL-адрес конечной точки и проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="72684-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="72684-108">Соединители API можно использовать на определенном шаге в потоке пользователей, чтобы повлиять на выполнение потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="72684-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="72684-109">Например, ответ API может заблокировать регистрацию пользователя, показать ошибку проверки ввода или переписать собранные атрибуты пользователя.</span><span class="sxs-lookup"><span data-stu-id="72684-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="72684-110">Используйте [API b2xIdentityUserFlow](b2xidentityuserflow.md) для использования соединителю API из потока пользователей самообслуживания внешних удостоверений.</span><span class="sxs-lookup"><span data-stu-id="72684-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="72684-111">Методы</span><span class="sxs-lookup"><span data-stu-id="72684-111">Methods</span></span>

|<span data-ttu-id="72684-112">Метод</span><span class="sxs-lookup"><span data-stu-id="72684-112">Method</span></span>|<span data-ttu-id="72684-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="72684-113">Return type</span></span>|<span data-ttu-id="72684-114">Описание</span><span class="sxs-lookup"><span data-stu-id="72684-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72684-115">Список</span><span class="sxs-lookup"><span data-stu-id="72684-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="72684-116">[коллекция identityApiConnector](identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="72684-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="72684-117">Получить список соединителов API</span><span class="sxs-lookup"><span data-stu-id="72684-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="72684-118">Создание</span><span class="sxs-lookup"><span data-stu-id="72684-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="72684-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="72684-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="72684-120">Создание нового соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="72684-120">Create a new API connector.</span></span> |
|<span data-ttu-id="72684-121">[получение](../api/identityapiconnector-get.md);</span><span class="sxs-lookup"><span data-stu-id="72684-121">[Get](../api/identityapiconnector-get.md)</span></span>|[<span data-ttu-id="72684-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="72684-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="72684-123">Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="72684-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="72684-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="72684-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="72684-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="72684-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="72684-126">Обновление свойств соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="72684-126">Update the properties of an API connector.</span></span>|
|<span data-ttu-id="72684-127">[удаление](../api/identityapiconnector-delete.md);</span><span class="sxs-lookup"><span data-stu-id="72684-127">[Delete](../api/identityapiconnector-delete.md)</span></span>|<span data-ttu-id="72684-128">Нет</span><span class="sxs-lookup"><span data-stu-id="72684-128">None</span></span>|<span data-ttu-id="72684-129">Удаление соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="72684-129">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="72684-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="72684-130">Properties</span></span>

|<span data-ttu-id="72684-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="72684-131">Property</span></span>|<span data-ttu-id="72684-132">Тип</span><span class="sxs-lookup"><span data-stu-id="72684-132">Type</span></span>|<span data-ttu-id="72684-133">Описание</span><span class="sxs-lookup"><span data-stu-id="72684-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72684-134">id</span><span class="sxs-lookup"><span data-stu-id="72684-134">id</span></span>|<span data-ttu-id="72684-135">String</span><span class="sxs-lookup"><span data-stu-id="72684-135">String</span></span>|<span data-ttu-id="72684-136">Случайно созданный ID соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="72684-136">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="72684-137">displayName</span><span class="sxs-lookup"><span data-stu-id="72684-137">displayName</span></span>|<span data-ttu-id="72684-138">String</span><span class="sxs-lookup"><span data-stu-id="72684-138">String</span></span>| <span data-ttu-id="72684-139">Имя соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="72684-139">The name of the API connector.</span></span> |
|<span data-ttu-id="72684-140">targetUrl</span><span class="sxs-lookup"><span data-stu-id="72684-140">targetUrl</span></span>|<span data-ttu-id="72684-141">String</span><span class="sxs-lookup"><span data-stu-id="72684-141">String</span></span>| <span data-ttu-id="72684-142">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="72684-142">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="72684-143">проверка подлинностиКонфигурация</span><span class="sxs-lookup"><span data-stu-id="72684-143">authenticationConfiguration</span></span>|[<span data-ttu-id="72684-144">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="72684-144">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="72684-145">Объект, описывая сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="72684-145">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="72684-146">В [настоящее время](basicauthentication.md) поддерживается только базовая проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="72684-146">Only [Basic authentication](basicauthentication.md) is supported at this time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72684-147">Связи</span><span class="sxs-lookup"><span data-stu-id="72684-147">Relationships</span></span>

<span data-ttu-id="72684-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72684-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72684-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="72684-149">JSON representation</span></span>

<span data-ttu-id="72684-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72684-150">The following is a JSON representation of the resource.</span></span>
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
