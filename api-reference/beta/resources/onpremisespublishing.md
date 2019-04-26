---
title: Тип ресурса Онпремисеспублишинг
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 8531a68ad56dad0f44ef8cd55e9fabeff47a6c2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341805"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="b7a2a-103">Тип ресурса Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="b7a2a-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="b7a2a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7a2a-104">Properties</span></span>
| <span data-ttu-id="b7a2a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7a2a-105">Property</span></span>     | <span data-ttu-id="b7a2a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b7a2a-106">Type</span></span>   |<span data-ttu-id="b7a2a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b7a2a-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7a2a-108">Кустомдомаинцертификате</span><span class="sxs-lookup"><span data-stu-id="b7a2a-108">customDomainCertificate</span></span>|<span data-ttu-id="b7a2a-109">String</span><span class="sxs-lookup"><span data-stu-id="b7a2a-109">String</span></span>|<span data-ttu-id="b7a2a-110">Сведения о сертификате, связанном с приложением при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="b7a2a-111">NULL при использовании домена по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="b7a2a-112">Екстерналаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="b7a2a-112">externalAuthenticationType</span></span>|<span data-ttu-id="b7a2a-113">String</span><span class="sxs-lookup"><span data-stu-id="b7a2a-113">String</span></span>|<span data-ttu-id="b7a2a-114">Detailed: параметры предварительной проверки подлинности для возможных значений `passthru`приложения `aadPreAuthentication`:,.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="b7a2a-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="b7a2a-115">externalUrl</span></span>|<span data-ttu-id="b7a2a-116">String</span><span class="sxs-lookup"><span data-stu-id="b7a2a-116">String</span></span>|<span data-ttu-id="b7a2a-117">Опубликованный внешний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-117">The published external url for the application.</span></span> <span data-ttu-id="b7a2a-118">Напримерhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="b7a2a-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="b7a2a-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="b7a2a-119">internalUrl</span></span>|<span data-ttu-id="b7a2a-120">String</span><span class="sxs-lookup"><span data-stu-id="b7a2a-120">String</span></span>|<span data-ttu-id="b7a2a-121">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-121">The internal url of the application.</span></span> <span data-ttu-id="b7a2a-122">Напримерhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="b7a2a-122">For example https://intranet/</span></span> |
|<span data-ttu-id="b7a2a-123">Исонпремпублишинженаблед</span><span class="sxs-lookup"><span data-stu-id="b7a2a-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="b7a2a-124">Логический</span><span class="sxs-lookup"><span data-stu-id="b7a2a-124">Boolean</span></span>|<span data-ttu-id="b7a2a-125">Указывает, выполняется ли публикация приложения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="b7a2a-126">Аппликатионсервертимеаут</span><span class="sxs-lookup"><span data-stu-id="b7a2a-126">applicationServerTimeout</span></span>|<span data-ttu-id="b7a2a-127">String</span><span class="sxs-lookup"><span data-stu-id="b7a2a-127">String</span></span>|<span data-ttu-id="b7a2a-128">Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="b7a2a-129">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="b7a2a-130">Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="b7a2a-131">Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".</span><span class="sxs-lookup"><span data-stu-id="b7a2a-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="b7a2a-132">Истранслатехоссеадеренаблед</span><span class="sxs-lookup"><span data-stu-id="b7a2a-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="b7a2a-133">Логический</span><span class="sxs-lookup"><span data-stu-id="b7a2a-133">Boolean</span></span>|<span data-ttu-id="b7a2a-134">Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="b7a2a-135">Сюда входит настройка правильного сайта для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7a2a-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7a2a-136">JSON representation</span></span>

<span data-ttu-id="b7a2a-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7a2a-137">Here is a JSON representation of the resource.</span></span>

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
