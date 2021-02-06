---
title: Тип ресурса apiApplication
description: Указывает параметры для приложения веб-API.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 499cc3d86ccab8706838dd3cf883b879d8bcea12
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137104"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="440d8-103">Тип ресурса apiApplication</span><span class="sxs-lookup"><span data-stu-id="440d8-103">apiApplication resource type</span></span>

<span data-ttu-id="440d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="440d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="440d8-105">Задает параметры приложения, реализующего веб-API.</span><span class="sxs-lookup"><span data-stu-id="440d8-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="440d8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="440d8-106">Properties</span></span>

| <span data-ttu-id="440d8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="440d8-107">Property</span></span> | <span data-ttu-id="440d8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="440d8-108">Type</span></span> | <span data-ttu-id="440d8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="440d8-109">Description</span></span> |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| <span data-ttu-id="440d8-110">Логический</span><span class="sxs-lookup"><span data-stu-id="440d8-110">Boolean</span></span> | <span data-ttu-id="440d8-111">Если имеет значение true, приложение может использовать сопоставление утверждений без указания пользовательского ключа подписи.</span><span class="sxs-lookup"><span data-stu-id="440d8-111">When true, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|`knownClientApplications`| <span data-ttu-id="440d8-112">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="440d8-112">Guid collection</span></span> |<span data-ttu-id="440d8-113">Используется для согласования согласия, если у вас есть решение, которое содержит две части: клиентского приложения и настраиваемого веб-приложения API.</span><span class="sxs-lookup"><span data-stu-id="440d8-113">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="440d8-114">Если для appID клиентского приложения задано это значение, пользователь дает согласие только один раз для клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="440d8-114">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="440d8-115">Azure AD знает, что предоставление согласия клиенту означает неявное согласие на веб-API и автоматическое предоставление обоих API-api- и автоматических условий для обоих API.</span><span class="sxs-lookup"><span data-stu-id="440d8-115">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="440d8-116">Клиент и приложение веб-API должны быть зарегистрированы в одном клиенте.</span><span class="sxs-lookup"><span data-stu-id="440d8-116">Both the client and the web API app must be registered in the same tenant.</span></span>|
|`oauth2PermissionScopes`| <span data-ttu-id="440d8-117">Коллекция [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="440d8-117">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="440d8-118">Определение делегирования разрешений, представляемого веб-API, представленным регистрацией этого приложения.</span><span class="sxs-lookup"><span data-stu-id="440d8-118">The definition of the delegated permissions exposed by the web API represented by this application registration.</span></span> <span data-ttu-id="440d8-119">Эти делегированные разрешения могут запрашиваться клиентской приложением и предоставляться пользователями или администраторами во время получения согласия.</span><span class="sxs-lookup"><span data-stu-id="440d8-119">These delegated permissions may be requested by a client application, and may be granted by users or administrators during consent.</span></span> <span data-ttu-id="440d8-120">Делегирование разрешений иногда называется областью OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="440d8-120">Delegated permissions are sometimes referred to as OAuth 2.0 scopes.</span></span> |
|`preAuthorizedApplications`| <span data-ttu-id="440d8-121">[Коллекция preAuthorizedApplication](preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="440d8-121">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="440d8-122">Перечисляет клиентские приложения, предварительно авторизованные с помощью указанных делегированных разрешений на доступ к API этого приложения.</span><span class="sxs-lookup"><span data-stu-id="440d8-122">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="440d8-123">Пользователи не обязаны соглашаться с любым предварительно авторизованном приложением (для указанных разрешений).</span><span class="sxs-lookup"><span data-stu-id="440d8-123">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="440d8-124">Однако любые дополнительные разрешения, не указанные в preAuthorizedApplications (например, запрашиваются с помощью добавимого согласия), требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="440d8-124">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|`requestedAccessTokenVersion`| <span data-ttu-id="440d8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="440d8-125">Int32</span></span> | <span data-ttu-id="440d8-126">Указывает версию маркера доступа, ожидаемую этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="440d8-126">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="440d8-127">Это изменяет версию и формат JWT независимо от конечной точки или клиента, используемых для запроса маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="440d8-127">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="440d8-128">Используемая конечная точка версии 1.0 или 2.0 выбирается клиентом и влияет только на версию id_tokens.</span><span class="sxs-lookup"><span data-stu-id="440d8-128">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="440d8-129">Ресурсы необходимо явно настроить, чтобы `requestedAccessTokenVersion` указать поддерживаемый формат маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="440d8-129">Resources need to explicitly configure `requestedAccessTokenVersion` to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="440d8-130">Возможные `requestedAccessTokenVersion` значения: `1` `2` , или `null` .</span><span class="sxs-lookup"><span data-stu-id="440d8-130">Possible values for `requestedAccessTokenVersion` are `1`, `2`, or `null`.</span></span> <span data-ttu-id="440d8-131">Если значение за этим значением, значение по умолчанию соответствует конечной точке `null` `1` 1.0.</span><span class="sxs-lookup"><span data-stu-id="440d8-131">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="440d8-132">Если `signInAudience` в приложении настроено значение, значение `AzureADandPersonalMicrosoftAccount` этого свойства должно быть `2`</span><span class="sxs-lookup"><span data-stu-id="440d8-132">If `signInAudience` on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="440d8-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="440d8-133">JSON representation</span></span>

<span data-ttu-id="440d8-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="440d8-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "acceptMappedClaims": true,
  "knownClientApplications": ["Guid"],
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "requestedAccessTokenVersion": 2
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


