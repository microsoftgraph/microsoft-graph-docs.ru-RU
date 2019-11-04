---
title: Тип ресурса Апиаппликатион
description: Задает параметры для приложения веб-API.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 85e9c5f62182b1dd7666117c6fcf42743ccc1e8e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939161"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="5577b-103">Тип ресурса Апиаппликатион</span><span class="sxs-lookup"><span data-stu-id="5577b-103">apiApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5577b-104">Задает параметры для приложения, реализующего веб-API.</span><span class="sxs-lookup"><span data-stu-id="5577b-104">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="5577b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5577b-105">Properties</span></span>

| <span data-ttu-id="5577b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5577b-106">Property</span></span> | <span data-ttu-id="5577b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5577b-107">Type</span></span> | <span data-ttu-id="5577b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5577b-108">Description</span></span> |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| <span data-ttu-id="5577b-109">Логический</span><span class="sxs-lookup"><span data-stu-id="5577b-109">Boolean</span></span> | <span data-ttu-id="5577b-110">Если значение равно true, приложение сможет использовать сопоставление утверждений без указания пользовательского ключа подписи.</span><span class="sxs-lookup"><span data-stu-id="5577b-110">When true, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|`knownClientApplications`| <span data-ttu-id="5577b-111">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="5577b-111">Guid collection</span></span> |<span data-ttu-id="5577b-112">Используется для предоставления согласия при наличии решения, содержащего две части: клиентское приложение и пользовательское приложение веб-API.</span><span class="sxs-lookup"><span data-stu-id="5577b-112">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="5577b-113">Если задать для appID для клиентского приложения это значение, пользователь только один раз отправляется в клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="5577b-113">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="5577b-114">В Azure AD известно, что при отправке клиенту неявным образом отправляются в веб-API и автоматически подготавливает субъекты-службы для обоих API одновременно.</span><span class="sxs-lookup"><span data-stu-id="5577b-114">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="5577b-115">Клиентское приложение и веб-API должны быть зарегистрированы в одном клиенте.</span><span class="sxs-lookup"><span data-stu-id="5577b-115">Both the client and the web API app must be registered in the same tenant.</span></span>|
|`oauth2PermissionScopes`| <span data-ttu-id="5577b-116">Коллекция [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="5577b-116">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="5577b-117">Коллекция областей разрешений OAuth 2,0, предоставляемых приложением веб-API (ресурсом) для клиентских приложений.</span><span class="sxs-lookup"><span data-stu-id="5577b-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="5577b-118">Эти области разрешений могут быть назначены клиентским приложениям во время согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="5577b-118">These permission scopes may be granted to client applications during consent.</span></span> |
|`preAuthorizedApplications`| <span data-ttu-id="5577b-119">Коллекция [preAuthorizedApplication](preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="5577b-119">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="5577b-120">Перечисляет клиентские приложения, которые предварительно авторизованы с указанными делегированными разрешениями для доступа к API этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5577b-120">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="5577b-121">Пользователям не требуется согласие с какими-либо из предварительно разрешенных приложений (для указанных разрешений).</span><span class="sxs-lookup"><span data-stu-id="5577b-121">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="5577b-122">Однако все дополнительные разрешения, не указанные в Преаусоризедаппликатионс (например, по запросу добавочного согласия), требуют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="5577b-122">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|`requestedAccessTokenVersion`| <span data-ttu-id="5577b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5577b-123">Int32</span></span> | <span data-ttu-id="5577b-124">Указывает версию маркера доступа, ожидаемую этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="5577b-124">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="5577b-125">При этом изменяется версия и формат JWT, созданного независимо от конечной точки или клиента, используемого для запроса маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="5577b-125">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="5577b-126">Используемая конечная точка, v 1.0 или v 2.0, выбирается клиентом и влияет только на версию id_tokens.</span><span class="sxs-lookup"><span data-stu-id="5577b-126">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="5577b-127">Ресурсы необходимо явно настроить `requestedAccessTokenVersion` , чтобы указать поддерживаемый формат маркеров доступа.</span><span class="sxs-lookup"><span data-stu-id="5577b-127">Resources need to explicitly configure `requestedAccessTokenVersion` to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="5577b-128">Возможные значения `requestedAccessTokenVersion` : `1`, `2`, или. `null`</span><span class="sxs-lookup"><span data-stu-id="5577b-128">Possible values for `requestedAccessTokenVersion` are `1`, `2`, or `null`.</span></span> <span data-ttu-id="5577b-129">Если задано `null`значение, по умолчанию используется `1`значение, соответствующее конечной точке версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="5577b-129">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="5577b-130">Если `signInAudience` для приложения задано значение `AzureADandPersonalMicrosoftAccount`, то значение этого свойства должно быть`2`</span><span class="sxs-lookup"><span data-stu-id="5577b-130">If `signInAudience` on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5577b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5577b-131">JSON representation</span></span>
<span data-ttu-id="5577b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5577b-132">Here is a JSON representation of the resource.</span></span>

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
