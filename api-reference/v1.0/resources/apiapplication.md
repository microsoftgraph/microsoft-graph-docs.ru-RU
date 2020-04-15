---
title: Тип ресурса Апиаппликатион
description: Задает параметры для приложения веб-API.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 91c37d5f9eb6dc5c6db7bd89bfb57ae116aad40e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439668"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="1bed0-103">Тип ресурса Апиаппликатион</span><span class="sxs-lookup"><span data-stu-id="1bed0-103">apiApplication resource type</span></span>

<span data-ttu-id="1bed0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bed0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bed0-105">Задает параметры приложения, реализующего веб-API.</span><span class="sxs-lookup"><span data-stu-id="1bed0-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="1bed0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bed0-106">Properties</span></span>

| <span data-ttu-id="1bed0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bed0-107">Property</span></span> | <span data-ttu-id="1bed0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1bed0-108">Type</span></span> | <span data-ttu-id="1bed0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1bed0-109">Description</span></span> |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| <span data-ttu-id="1bed0-110">Логический</span><span class="sxs-lookup"><span data-stu-id="1bed0-110">Boolean</span></span> | <span data-ttu-id="1bed0-111">Если значение равно true, приложение сможет использовать сопоставление утверждений без указания пользовательского ключа подписи.</span><span class="sxs-lookup"><span data-stu-id="1bed0-111">When true, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|`knownClientApplications`| <span data-ttu-id="1bed0-112">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="1bed0-112">Guid collection</span></span> |<span data-ttu-id="1bed0-113">Используется для предоставления согласия при наличии решения, содержащего две части: клиентское приложение и пользовательское приложение веб-API.</span><span class="sxs-lookup"><span data-stu-id="1bed0-113">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="1bed0-114">Если задать для appID для клиентского приложения это значение, пользователь только один раз отправляется в клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="1bed0-114">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="1bed0-115">В Azure AD известно, что при отправке клиенту неявным образом отправляются в веб-API и автоматически подготавливает субъекты-службы для обоих API одновременно.</span><span class="sxs-lookup"><span data-stu-id="1bed0-115">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="1bed0-116">Клиентское приложение и веб-API должны быть зарегистрированы в одном клиенте.</span><span class="sxs-lookup"><span data-stu-id="1bed0-116">Both the client and the web API app must be registered in the same tenant.</span></span>|
|`oauth2PermissionScopes`| <span data-ttu-id="1bed0-117">Коллекция [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="1bed0-117">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="1bed0-118">Коллекция областей разрешений OAuth 2,0, предоставляемых приложением веб-API (ресурсом) для клиентских приложений.</span><span class="sxs-lookup"><span data-stu-id="1bed0-118">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="1bed0-119">Эти области разрешений могут быть назначены клиентским приложениям во время согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="1bed0-119">These permission scopes may be granted to client applications during consent.</span></span> |
|`preAuthorizedApplications`| <span data-ttu-id="1bed0-120">Коллекция [preAuthorizedApplication](preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="1bed0-120">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="1bed0-121">Перечисляет клиентские приложения, которые предварительно авторизованы с указанными делегированными разрешениями для доступа к API этого приложения.</span><span class="sxs-lookup"><span data-stu-id="1bed0-121">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="1bed0-122">Пользователям не требуется согласие с какими-либо из предварительно разрешенных приложений (для указанных разрешений).</span><span class="sxs-lookup"><span data-stu-id="1bed0-122">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="1bed0-123">Однако все дополнительные разрешения, не указанные в Преаусоризедаппликатионс (например, по запросу добавочного согласия), требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="1bed0-123">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|`requestedAccessTokenVersion`| <span data-ttu-id="1bed0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="1bed0-124">Int32</span></span> | <span data-ttu-id="1bed0-125">Указывает версию маркера доступа, ожидаемую этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="1bed0-125">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="1bed0-126">При этом изменяется версия и формат JWT, созданного независимо от конечной точки или клиента, используемого для запроса маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="1bed0-126">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="1bed0-127">Используемая конечная точка, v 1.0 или v 2.0, выбирается клиентом и влияет только на версию id_tokens.</span><span class="sxs-lookup"><span data-stu-id="1bed0-127">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="1bed0-128">Ресурсы необходимо явно настроить `requestedAccessTokenVersion` , чтобы указать поддерживаемый формат маркеров доступа.</span><span class="sxs-lookup"><span data-stu-id="1bed0-128">Resources need to explicitly configure `requestedAccessTokenVersion` to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="1bed0-129">Возможные значения `requestedAccessTokenVersion` : `1`, `2`, или. `null`</span><span class="sxs-lookup"><span data-stu-id="1bed0-129">Possible values for `requestedAccessTokenVersion` are `1`, `2`, or `null`.</span></span> <span data-ttu-id="1bed0-130">Если задано `null`значение, по умолчанию используется `1`значение, соответствующее конечной точке версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="1bed0-130">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="1bed0-131">Если `signInAudience` для приложения задано значение `AzureADandPersonalMicrosoftAccount`, то значение этого свойства должно быть`2`</span><span class="sxs-lookup"><span data-stu-id="1bed0-131">If `signInAudience` on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bed0-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bed0-132">JSON representation</span></span>
<span data-ttu-id="1bed0-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bed0-133">Here is a JSON representation of the resource.</span></span>

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
