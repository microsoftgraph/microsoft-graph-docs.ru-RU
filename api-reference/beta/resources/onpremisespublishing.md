---
title: Тип ресурса onPremisesPublishing
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 30ff6908a42a690e07d71b5d0c62fcb22dea3c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842541"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="5b54a-103">Тип ресурса onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="5b54a-103">onPremisesPublishing resource type</span></span>

> <span data-ttu-id="5b54a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b54a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b54a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b54a-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="5b54a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b54a-106">Properties</span></span>
| <span data-ttu-id="5b54a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b54a-107">Property</span></span>     | <span data-ttu-id="5b54a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5b54a-108">Type</span></span>   |<span data-ttu-id="5b54a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5b54a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b54a-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="5b54a-110">customDomainCertificate</span></span>|<span data-ttu-id="5b54a-111">Строка</span><span class="sxs-lookup"><span data-stu-id="5b54a-111">String</span></span>|<span data-ttu-id="5b54a-112">Сведения о сертификате, связанных с приложением, при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="5b54a-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="5b54a-113">Использование домена по умолчанию значение NULL.</span><span class="sxs-lookup"><span data-stu-id="5b54a-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="5b54a-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="5b54a-114">externalAuthenticationType</span></span>|<span data-ttu-id="5b54a-115">Строка</span><span class="sxs-lookup"><span data-stu-id="5b54a-115">String</span></span>|<span data-ttu-id="5b54a-116">Дополнительные сведения об значение предварительной проверки подлинности для приложения возможными значениями являются: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="5b54a-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="5b54a-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="5b54a-117">externalUrl</span></span>|<span data-ttu-id="5b54a-118">Строка</span><span class="sxs-lookup"><span data-stu-id="5b54a-118">String</span></span>|<span data-ttu-id="5b54a-119">Опубликованные внешний URL-адрес для приложения.</span><span class="sxs-lookup"><span data-stu-id="5b54a-119">The published external url for the application.</span></span> <span data-ttu-id="5b54a-120">Напримерhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="5b54a-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="5b54a-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="5b54a-121">internalUrl</span></span>|<span data-ttu-id="5b54a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5b54a-122">String</span></span>|<span data-ttu-id="5b54a-123">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="5b54a-123">The internal url of the application.</span></span> <span data-ttu-id="5b54a-124">Напримерhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="5b54a-124">For example https://intranet/</span></span> |
|<span data-ttu-id="5b54a-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="5b54a-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="5b54a-126">Логический</span><span class="sxs-lookup"><span data-stu-id="5b54a-126">Boolean</span></span>|<span data-ttu-id="5b54a-127">Указывает, если приложение публикуется в настоящее время или нет.</span><span class="sxs-lookup"><span data-stu-id="5b54a-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="5b54a-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="5b54a-128">applicationServerTimeout</span></span>|<span data-ttu-id="5b54a-129">Строка</span><span class="sxs-lookup"><span data-stu-id="5b54a-129">String</span></span>|<span data-ttu-id="5b54a-130">Во время выполнения соединитель будет ожидать ответа из базы данных приложения до закрытия подключения.</span><span class="sxs-lookup"><span data-stu-id="5b54a-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="5b54a-131">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="5b54a-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="5b54a-132">Использование `long` Если сервер принимает более 60 75 секунд отвечать на запросы.</span><span class="sxs-lookup"><span data-stu-id="5b54a-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="5b54a-133">Также попробуйте `long` Если вы не можете получить доступ к приложению и состояние ошибки «Время ожидания базы данных».</span><span class="sxs-lookup"><span data-stu-id="5b54a-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="5b54a-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="5b54a-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="5b54a-135">Логический</span><span class="sxs-lookup"><span data-stu-id="5b54a-135">Boolean</span></span>|<span data-ttu-id="5b54a-136">Указывает, если приложение следует перевести URL-адреса в заголовке ответа.</span><span class="sxs-lookup"><span data-stu-id="5b54a-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="5b54a-137">Этот компонент включает Установка правильное веб-узла для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="5b54a-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b54a-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b54a-138">JSON representation</span></span>

<span data-ttu-id="5b54a-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b54a-139">Here is a JSON representation of the resource.</span></span>

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
