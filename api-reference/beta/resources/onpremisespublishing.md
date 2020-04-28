---
title: Тип ресурса Онпремисеспублишинг
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9395a2d51628ed6ffc8ed0049f73595e2c98ba7a
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200056"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="10698-103">Тип ресурса Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="10698-103">onPremisesPublishing resource type</span></span>

<span data-ttu-id="10698-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10698-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10698-105">Объект **онпремисеспублишинг** представляет набор свойств для публикации локального [приложения](application.md).</span><span class="sxs-lookup"><span data-stu-id="10698-105">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10698-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="10698-106">Properties</span></span>

| <span data-ttu-id="10698-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="10698-107">Property</span></span>|<span data-ttu-id="10698-108">Тип</span><span class="sxs-lookup"><span data-stu-id="10698-108">Type</span></span>|<span data-ttu-id="10698-109">Описание</span><span class="sxs-lookup"><span data-stu-id="10698-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10698-110">кустомдомаинцертификате</span><span class="sxs-lookup"><span data-stu-id="10698-110">customDomainCertificate</span></span>|<span data-ttu-id="10698-111">String</span><span class="sxs-lookup"><span data-stu-id="10698-111">String</span></span>|<span data-ttu-id="10698-112">Сведения о сертификате, связанном с приложением при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="10698-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="10698-113">NULL при использовании домена по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="10698-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="10698-114">екстерналаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="10698-114">externalAuthenticationType</span></span>|<span data-ttu-id="10698-115">String</span><span class="sxs-lookup"><span data-stu-id="10698-115">String</span></span>|<span data-ttu-id="10698-116">Detailed: параметры предварительной проверки подлинности для возможных значений `passthru`приложения `aadPreAuthentication`:,.</span><span class="sxs-lookup"><span data-stu-id="10698-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="10698-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="10698-117">externalUrl</span></span>|<span data-ttu-id="10698-118">String</span><span class="sxs-lookup"><span data-stu-id="10698-118">String</span></span>|<span data-ttu-id="10698-119">Опубликованный внешний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="10698-119">The published external url for the application.</span></span> <span data-ttu-id="10698-120">Напримерhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="10698-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="10698-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="10698-121">internalUrl</span></span>|<span data-ttu-id="10698-122">String</span><span class="sxs-lookup"><span data-stu-id="10698-122">String</span></span>|<span data-ttu-id="10698-123">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="10698-123">The internal url of the application.</span></span> <span data-ttu-id="10698-124">Напримерhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="10698-124">For example https://intranet/</span></span> |
|<span data-ttu-id="10698-125">исонпремпублишинженаблед</span><span class="sxs-lookup"><span data-stu-id="10698-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="10698-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="10698-126">Boolean</span></span>|<span data-ttu-id="10698-127">Указывает, выполняется ли публикация приложения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="10698-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="10698-128">аппликатионсервертимеаут</span><span class="sxs-lookup"><span data-stu-id="10698-128">applicationServerTimeout</span></span>|<span data-ttu-id="10698-129">String</span><span class="sxs-lookup"><span data-stu-id="10698-129">String</span></span>|<span data-ttu-id="10698-130">Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения.</span><span class="sxs-lookup"><span data-stu-id="10698-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="10698-131">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="10698-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="10698-132">Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы.</span><span class="sxs-lookup"><span data-stu-id="10698-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="10698-133">Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".</span><span class="sxs-lookup"><span data-stu-id="10698-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="10698-134">истранслатехоссеадеренаблед</span><span class="sxs-lookup"><span data-stu-id="10698-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="10698-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="10698-135">Boolean</span></span>|<span data-ttu-id="10698-136">Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа.</span><span class="sxs-lookup"><span data-stu-id="10698-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="10698-137">Сюда входит настройка правильного сайта для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="10698-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10698-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10698-138">JSON representation</span></span>

<span data-ttu-id="10698-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10698-139">Here is a JSON representation of the resource.</span></span>

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
