---
title: Тип ресурса Онпремисеспублишинг
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: db81ef2c61142edb0d3ca58a67b34c7da34e71f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522216"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="2ee73-103">Тип ресурса Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="2ee73-103">onPremisesPublishing resource type</span></span>

<span data-ttu-id="2ee73-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ee73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ee73-105">Объект **онпремисеспублишинг** представляет набор свойств для публикации локального [приложения](application.md).</span><span class="sxs-lookup"><span data-stu-id="2ee73-105">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2ee73-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ee73-106">Properties</span></span>

| <span data-ttu-id="2ee73-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ee73-107">Property</span></span>|<span data-ttu-id="2ee73-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2ee73-108">Type</span></span>|<span data-ttu-id="2ee73-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2ee73-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ee73-110">кустомдомаинцертификате</span><span class="sxs-lookup"><span data-stu-id="2ee73-110">customDomainCertificate</span></span>|<span data-ttu-id="2ee73-111">String</span><span class="sxs-lookup"><span data-stu-id="2ee73-111">String</span></span>|<span data-ttu-id="2ee73-112">Сведения о сертификате, связанном с приложением при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="2ee73-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="2ee73-113">NULL при использовании домена по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2ee73-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="2ee73-114">екстерналаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="2ee73-114">externalAuthenticationType</span></span>|<span data-ttu-id="2ee73-115">String</span><span class="sxs-lookup"><span data-stu-id="2ee73-115">String</span></span>|<span data-ttu-id="2ee73-116">Detailed: параметры предварительной проверки подлинности для возможных значений `passthru`приложения `aadPreAuthentication`:,.</span><span class="sxs-lookup"><span data-stu-id="2ee73-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="2ee73-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="2ee73-117">externalUrl</span></span>|<span data-ttu-id="2ee73-118">String</span><span class="sxs-lookup"><span data-stu-id="2ee73-118">String</span></span>|<span data-ttu-id="2ee73-119">Опубликованный внешний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="2ee73-119">The published external url for the application.</span></span> <span data-ttu-id="2ee73-120">Напримерhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="2ee73-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="2ee73-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="2ee73-121">internalUrl</span></span>|<span data-ttu-id="2ee73-122">String</span><span class="sxs-lookup"><span data-stu-id="2ee73-122">String</span></span>|<span data-ttu-id="2ee73-123">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="2ee73-123">The internal url of the application.</span></span> <span data-ttu-id="2ee73-124">Напримерhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="2ee73-124">For example https://intranet/</span></span> |
|<span data-ttu-id="2ee73-125">исонпремпублишинженаблед</span><span class="sxs-lookup"><span data-stu-id="2ee73-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="2ee73-126">Логический</span><span class="sxs-lookup"><span data-stu-id="2ee73-126">Boolean</span></span>|<span data-ttu-id="2ee73-127">Указывает, выполняется ли публикация приложения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="2ee73-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="2ee73-128">аппликатионсервертимеаут</span><span class="sxs-lookup"><span data-stu-id="2ee73-128">applicationServerTimeout</span></span>|<span data-ttu-id="2ee73-129">String</span><span class="sxs-lookup"><span data-stu-id="2ee73-129">String</span></span>|<span data-ttu-id="2ee73-130">Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения.</span><span class="sxs-lookup"><span data-stu-id="2ee73-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="2ee73-131">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="2ee73-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="2ee73-132">Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы.</span><span class="sxs-lookup"><span data-stu-id="2ee73-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="2ee73-133">Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".</span><span class="sxs-lookup"><span data-stu-id="2ee73-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="2ee73-134">истранслатехоссеадеренаблед</span><span class="sxs-lookup"><span data-stu-id="2ee73-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="2ee73-135">Логический</span><span class="sxs-lookup"><span data-stu-id="2ee73-135">Boolean</span></span>|<span data-ttu-id="2ee73-136">Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа.</span><span class="sxs-lookup"><span data-stu-id="2ee73-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="2ee73-137">Сюда входит настройка правильного сайта для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="2ee73-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ee73-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ee73-138">JSON representation</span></span>

<span data-ttu-id="2ee73-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ee73-139">Here is a JSON representation of the resource.</span></span>

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
2019-02-04 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
