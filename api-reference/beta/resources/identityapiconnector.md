---
title: Тип ресурса identityApiConnector
description: Представляет соединители API в клиенте Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e5b3c10e6a03c4868e010f8f62f0f073ce37ca61
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161651"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="ac0f0-103">Тип ресурса identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ac0f0-103">identityApiConnector resource type</span></span>

<span data-ttu-id="ac0f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac0f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac0f0-105">Представляет соединители API в клиентах Azure Active Directory (Azure AD) и Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="ac0f0-106">Соединитель API, используемый при самостоятельной регистрации внешних удостоверений Azure AD и потоках регистрации пользователей Azure AD B2C, позволяет вызывать API во время выполнения пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="ac0f0-107">Соединителение API предоставляет сведения, необходимые для вызова API, включая URL-адрес конечной точки и проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="ac0f0-108">Соединители API можно использовать на определенном этапе пользовательского потока, чтобы повлиять на выполнение пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="ac0f0-109">Например, ответ API может блокировать регистрацию пользователя, показывать ошибку проверки ввода или переописывать собранные пользователем атрибуты.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="ac0f0-110">Используйте API [b2xIdentityUserFlow](b2xidentityuserflow.md) для использования соединителю API из пользовательского потока самостоятельной регистрации внешних удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="ac0f0-111">Методы</span><span class="sxs-lookup"><span data-stu-id="ac0f0-111">Methods</span></span>

|<span data-ttu-id="ac0f0-112">Метод</span><span class="sxs-lookup"><span data-stu-id="ac0f0-112">Method</span></span>|<span data-ttu-id="ac0f0-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="ac0f0-113">Return type</span></span>|<span data-ttu-id="ac0f0-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ac0f0-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac0f0-115">Список</span><span class="sxs-lookup"><span data-stu-id="ac0f0-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="ac0f0-116">[Коллекция identityApiConnector](identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f0-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="ac0f0-117">Получить список соединителов API</span><span class="sxs-lookup"><span data-stu-id="ac0f0-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="ac0f0-118">Создание</span><span class="sxs-lookup"><span data-stu-id="ac0f0-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="ac0f0-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ac0f0-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="ac0f0-120">Создайте соединители API.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="ac0f0-121">Получение</span><span class="sxs-lookup"><span data-stu-id="ac0f0-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="ac0f0-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ac0f0-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="ac0f0-123">Чтение свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f0-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="ac0f0-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="ac0f0-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="ac0f0-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ac0f0-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="ac0f0-126">Обновление свойств соединители API.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-126">Update the properties of an API connector.</span></span>|
|<span data-ttu-id="ac0f0-127">[удаление](../api/identityapiconnector-delete.md);</span><span class="sxs-lookup"><span data-stu-id="ac0f0-127">[Delete](../api/identityapiconnector-delete.md)</span></span>|<span data-ttu-id="ac0f0-128">Нет</span><span class="sxs-lookup"><span data-stu-id="ac0f0-128">None</span></span>|<span data-ttu-id="ac0f0-129">Удаление соединители API.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-129">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac0f0-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac0f0-130">Properties</span></span>

|<span data-ttu-id="ac0f0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac0f0-131">Property</span></span>|<span data-ttu-id="ac0f0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ac0f0-132">Type</span></span>|<span data-ttu-id="ac0f0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ac0f0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac0f0-134">id</span><span class="sxs-lookup"><span data-stu-id="ac0f0-134">id</span></span>|<span data-ttu-id="ac0f0-135">String</span><span class="sxs-lookup"><span data-stu-id="ac0f0-135">String</span></span>|<span data-ttu-id="ac0f0-136">Случайным образом созданный ИД соединителю API.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-136">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="ac0f0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ac0f0-137">displayName</span></span>|<span data-ttu-id="ac0f0-138">String</span><span class="sxs-lookup"><span data-stu-id="ac0f0-138">String</span></span>| <span data-ttu-id="ac0f0-139">Имя соединители API.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-139">The name of the API connector.</span></span> |
|<span data-ttu-id="ac0f0-140">targetUrl</span><span class="sxs-lookup"><span data-stu-id="ac0f0-140">targetUrl</span></span>|<span data-ttu-id="ac0f0-141">String</span><span class="sxs-lookup"><span data-stu-id="ac0f0-141">String</span></span>| <span data-ttu-id="ac0f0-142">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-142">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="ac0f0-143">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac0f0-143">authenticationConfiguration</span></span>|[<span data-ttu-id="ac0f0-144">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="ac0f0-144">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="ac0f0-145">Объект, который описывает сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-145">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="ac0f0-146">В [настоящее время поддерживается](basicauthentication.md) только базовая проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-146">Only [Basic authentication](basicauthentication.md) is supported at this time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac0f0-147">Связи</span><span class="sxs-lookup"><span data-stu-id="ac0f0-147">Relationships</span></span>

<span data-ttu-id="ac0f0-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac0f0-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ac0f0-149">JSON representation</span></span>

<span data-ttu-id="ac0f0-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-150">The following is a JSON representation of the resource.</span></span>
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
