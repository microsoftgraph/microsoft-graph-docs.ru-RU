---
title: тип ресурса apiApplication
description: Указывает параметры приложения веб-API.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 1a01418fad74d48a1697bace91833d880a94f467
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955968"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="7083f-103">тип ресурса apiApplication</span><span class="sxs-lookup"><span data-stu-id="7083f-103">apiApplication resource type</span></span>

<span data-ttu-id="7083f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7083f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7083f-105">Задает параметры приложения, реализующего веб-API.</span><span class="sxs-lookup"><span data-stu-id="7083f-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="7083f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7083f-106">Properties</span></span>

| <span data-ttu-id="7083f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7083f-107">Property</span></span> | <span data-ttu-id="7083f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7083f-108">Type</span></span> | <span data-ttu-id="7083f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7083f-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7083f-110">acceptMappedClaims</span><span class="sxs-lookup"><span data-stu-id="7083f-110">acceptMappedClaims</span></span>| <span data-ttu-id="7083f-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="7083f-111">Boolean</span></span> | <span data-ttu-id="7083f-112">Когда , позволяет приложению использовать сопоставление утверждений `true` без указания пользовательского ключа подписи.</span><span class="sxs-lookup"><span data-stu-id="7083f-112">When `true`, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|<span data-ttu-id="7083f-113">knownClientApplications</span><span class="sxs-lookup"><span data-stu-id="7083f-113">knownClientApplications</span></span>| <span data-ttu-id="7083f-114">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="7083f-114">Guid collection</span></span> |<span data-ttu-id="7083f-115">Используется для согласования согласия, если у вас есть решение, которое содержит две части: клиентского приложения и настраиваемого веб-приложения API.</span><span class="sxs-lookup"><span data-stu-id="7083f-115">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="7083f-116">Если приложение клиентского приложения установлено к этому значению, пользователь только один раз соглашается на это приложение.</span><span class="sxs-lookup"><span data-stu-id="7083f-116">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="7083f-117">Azure AD знает, что согласие клиента означает неявное согласие на веб-API и автоматически предусматривает предоставление основных служб для обоих API одновременно.</span><span class="sxs-lookup"><span data-stu-id="7083f-117">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="7083f-118">Клиент и приложение веб-API должны быть зарегистрированы в одном клиенте.</span><span class="sxs-lookup"><span data-stu-id="7083f-118">Both the client and the web API app must be registered in the same tenant.</span></span>|
|<span data-ttu-id="7083f-119">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="7083f-119">oauth2PermissionScopes</span></span>| <span data-ttu-id="7083f-120">Коллекция [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="7083f-120">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="7083f-121">Определение делегирования разрешений, выставленных веб-API, представленного этой регистрацией приложений.</span><span class="sxs-lookup"><span data-stu-id="7083f-121">The definition of the delegated permissions exposed by the web API represented by this application registration.</span></span> <span data-ttu-id="7083f-122">Эти делегированные разрешения могут запрашиваться клиентской заявкой и могут предоставляться пользователями или администраторами во время согласия.</span><span class="sxs-lookup"><span data-stu-id="7083f-122">These delegated permissions may be requested by a client application, and may be granted by users or administrators during consent.</span></span> <span data-ttu-id="7083f-123">Делегирование разрешений иногда называется областью OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="7083f-123">Delegated permissions are sometimes referred to as OAuth 2.0 scopes.</span></span> |
|<span data-ttu-id="7083f-124">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="7083f-124">preAuthorizedApplications</span></span>| <span data-ttu-id="7083f-125">[коллекция preAuthorizedApplication](preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="7083f-125">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="7083f-126">Списки клиентских приложений, предварительно авторизованных с указанными делегированных разрешений на доступ к API этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7083f-126">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="7083f-127">Пользователи не обязаны соглашаться на любое предварительно авторизованного приложения (для указанных разрешений).</span><span class="sxs-lookup"><span data-stu-id="7083f-127">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="7083f-128">Однако для любых дополнительных разрешений, не указанных в preAuthorizedApplications (запрашивается, например, с помощью дополнительного согласия), потребуется согласие пользователя.</span><span class="sxs-lookup"><span data-stu-id="7083f-128">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|<span data-ttu-id="7083f-129">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="7083f-129">requestedAccessTokenVersion</span></span>| <span data-ttu-id="7083f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7083f-130">Int32</span></span> | <span data-ttu-id="7083f-131">Указывает версию маркера доступа, ожидаемую этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="7083f-131">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="7083f-132">Это меняет версию и формат JWT, выпускаемого независимо от конечной точки или клиента, используемого для запроса маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="7083f-132">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="7083f-133">Используемая конечная точка , v1.0 или v2.0, выбирается клиентом и влияет только на версию id_tokens.</span><span class="sxs-lookup"><span data-stu-id="7083f-133">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="7083f-134">Ресурсы должны явно настроить **запрашиваемыйAccessTokenVersion,** чтобы указать поддерживаемый формат маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="7083f-134">Resources need to explicitly configure **requestedAccessTokenVersion** to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="7083f-135">Возможные значения **для requestedAccessSTokenVersion** являются `1` , или `2` `null` .</span><span class="sxs-lookup"><span data-stu-id="7083f-135">Possible values for **requestedAccessTokenVersion** are `1`, `2`, or `null`.</span></span> <span data-ttu-id="7083f-136">Если значение такое, это значение по умолчанию соответствует конечной точке `null` `1` v1.0.</span><span class="sxs-lookup"><span data-stu-id="7083f-136">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="7083f-137">Если **signInAudience** в приложении настроен как, значение для `AzureADandPersonalMicrosoftAccount` этого свойства должно быть `2`</span><span class="sxs-lookup"><span data-stu-id="7083f-137">If **signInAudience** on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7083f-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7083f-138">JSON representation</span></span>

<span data-ttu-id="7083f-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7083f-139">Here is a JSON representation of the resource.</span></span>

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

