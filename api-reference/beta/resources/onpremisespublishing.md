---
title: Тип ресурса Онпремисеспублишинг
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1ee3b9cd98ae61bd6322ee49fede6310f78815a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966379"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="42345-103">Тип ресурса Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="42345-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42345-104">Объект **онпремисеспублишинг** представляет набор свойств для публикации локального [приложения](application.md).</span><span class="sxs-lookup"><span data-stu-id="42345-104">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="42345-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="42345-105">Properties</span></span>

| <span data-ttu-id="42345-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="42345-106">Property</span></span>|<span data-ttu-id="42345-107">Тип</span><span class="sxs-lookup"><span data-stu-id="42345-107">Type</span></span>|<span data-ttu-id="42345-108">Описание</span><span class="sxs-lookup"><span data-stu-id="42345-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42345-109">Кустомдомаинцертификате</span><span class="sxs-lookup"><span data-stu-id="42345-109">customDomainCertificate</span></span>|<span data-ttu-id="42345-110">String</span><span class="sxs-lookup"><span data-stu-id="42345-110">String</span></span>|<span data-ttu-id="42345-111">Сведения о сертификате, связанном с приложением при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="42345-111">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="42345-112">NULL при использовании домена по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42345-112">Null when using the default domain.</span></span>|
|<span data-ttu-id="42345-113">Екстерналаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="42345-113">externalAuthenticationType</span></span>|<span data-ttu-id="42345-114">String</span><span class="sxs-lookup"><span data-stu-id="42345-114">String</span></span>|<span data-ttu-id="42345-115">Detailed: параметры предварительной проверки подлинности для возможных значений `passthru`приложения `aadPreAuthentication`:,.</span><span class="sxs-lookup"><span data-stu-id="42345-115">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="42345-116">externalUrl</span><span class="sxs-lookup"><span data-stu-id="42345-116">externalUrl</span></span>|<span data-ttu-id="42345-117">String</span><span class="sxs-lookup"><span data-stu-id="42345-117">String</span></span>|<span data-ttu-id="42345-118">Опубликованный внешний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="42345-118">The published external url for the application.</span></span> <span data-ttu-id="42345-119">Напримерhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="42345-119">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="42345-120">internalUrl</span><span class="sxs-lookup"><span data-stu-id="42345-120">internalUrl</span></span>|<span data-ttu-id="42345-121">String</span><span class="sxs-lookup"><span data-stu-id="42345-121">String</span></span>|<span data-ttu-id="42345-122">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="42345-122">The internal url of the application.</span></span> <span data-ttu-id="42345-123">Напримерhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="42345-123">For example https://intranet/</span></span> |
|<span data-ttu-id="42345-124">Исонпремпублишинженаблед</span><span class="sxs-lookup"><span data-stu-id="42345-124">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="42345-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="42345-125">Boolean</span></span>|<span data-ttu-id="42345-126">Указывает, выполняется ли публикация приложения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="42345-126">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="42345-127">Аппликатионсервертимеаут</span><span class="sxs-lookup"><span data-stu-id="42345-127">applicationServerTimeout</span></span>|<span data-ttu-id="42345-128">String</span><span class="sxs-lookup"><span data-stu-id="42345-128">String</span></span>|<span data-ttu-id="42345-129">Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения.</span><span class="sxs-lookup"><span data-stu-id="42345-129">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="42345-130">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="42345-130">Possible values are `default`, `long`.</span></span> <span data-ttu-id="42345-131">Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы.</span><span class="sxs-lookup"><span data-stu-id="42345-131">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="42345-132">Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".</span><span class="sxs-lookup"><span data-stu-id="42345-132">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="42345-133">Истранслатехоссеадеренаблед</span><span class="sxs-lookup"><span data-stu-id="42345-133">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="42345-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="42345-134">Boolean</span></span>|<span data-ttu-id="42345-135">Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа.</span><span class="sxs-lookup"><span data-stu-id="42345-135">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="42345-136">Сюда входит настройка правильного сайта для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="42345-136">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42345-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42345-137">JSON representation</span></span>

<span data-ttu-id="42345-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42345-138">Here is a JSON representation of the resource.</span></span>

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
