---
title: Тип ресурса onPremisesPublishing
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: 8dba505347fc12d3c4a8521ebe32551d738dc4a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078692"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="021bc-103">Тип ресурса onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="021bc-103">onPremisesPublishing resource type</span></span>

> <span data-ttu-id="021bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="021bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="021bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="021bc-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="021bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="021bc-106">Properties</span></span>
| <span data-ttu-id="021bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="021bc-107">Property</span></span>     | <span data-ttu-id="021bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="021bc-108">Type</span></span>   |<span data-ttu-id="021bc-109">Description</span><span class="sxs-lookup"><span data-stu-id="021bc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="021bc-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="021bc-110">customDomainCertificate</span></span>|<span data-ttu-id="021bc-111">String</span><span class="sxs-lookup"><span data-stu-id="021bc-111">String</span></span>|<span data-ttu-id="021bc-112">Сведения о сертификате, связанных с приложением, при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="021bc-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="021bc-113">Использование домена по умолчанию значение NULL.</span><span class="sxs-lookup"><span data-stu-id="021bc-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="021bc-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="021bc-114">externalAuthenticationType</span></span>|<span data-ttu-id="021bc-115">String</span><span class="sxs-lookup"><span data-stu-id="021bc-115">String</span></span>|<span data-ttu-id="021bc-116">Дополнительные сведения об значение предварительной проверки подлинности для приложения возможными значениями являются: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="021bc-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="021bc-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="021bc-117">externalUrl</span></span>|<span data-ttu-id="021bc-118">String</span><span class="sxs-lookup"><span data-stu-id="021bc-118">String</span></span>|<span data-ttu-id="021bc-119">Опубликованные внешний URL-адрес для приложения.</span><span class="sxs-lookup"><span data-stu-id="021bc-119">The published external url for the application.</span></span> <span data-ttu-id="021bc-120">Напримерhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="021bc-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="021bc-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="021bc-121">internalUrl</span></span>|<span data-ttu-id="021bc-122">String</span><span class="sxs-lookup"><span data-stu-id="021bc-122">String</span></span>|<span data-ttu-id="021bc-123">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="021bc-123">The internal url of the application.</span></span> <span data-ttu-id="021bc-124">Напримерhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="021bc-124">For example https://intranet/</span></span> |
|<span data-ttu-id="021bc-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="021bc-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="021bc-126">Логический</span><span class="sxs-lookup"><span data-stu-id="021bc-126">Boolean</span></span>|<span data-ttu-id="021bc-127">Указывает, если приложение публикуется в настоящее время или нет.</span><span class="sxs-lookup"><span data-stu-id="021bc-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="021bc-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="021bc-128">applicationServerTimeout</span></span>|<span data-ttu-id="021bc-129">String</span><span class="sxs-lookup"><span data-stu-id="021bc-129">String</span></span>|<span data-ttu-id="021bc-130">Во время выполнения соединитель будет ожидать ответа из базы данных приложения до закрытия подключения.</span><span class="sxs-lookup"><span data-stu-id="021bc-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="021bc-131">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="021bc-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="021bc-132">Использование `long` Если сервер принимает более 60 75 секунд отвечать на запросы.</span><span class="sxs-lookup"><span data-stu-id="021bc-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="021bc-133">Также попробуйте `long` Если вы не можете получить доступ к приложению и состояние ошибки «Время ожидания базы данных».</span><span class="sxs-lookup"><span data-stu-id="021bc-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="021bc-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="021bc-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="021bc-135">Логический</span><span class="sxs-lookup"><span data-stu-id="021bc-135">Boolean</span></span>|<span data-ttu-id="021bc-136">Указывает, если приложение следует перевести URL-адреса в заголовке ответа.</span><span class="sxs-lookup"><span data-stu-id="021bc-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="021bc-137">Этот компонент включает Установка правильное веб-узла для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="021bc-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="021bc-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="021bc-138">JSON representation</span></span>

<span data-ttu-id="021bc-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="021bc-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
