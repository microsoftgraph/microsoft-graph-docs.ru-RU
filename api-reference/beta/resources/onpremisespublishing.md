---
title: Тип ресурса Онпремисеспублишинг
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568869"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="b4e4f-103">Тип ресурса Онпремисеспублишинг</span><span class="sxs-lookup"><span data-stu-id="b4e4f-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="b4e4f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4e4f-104">Properties</span></span>
| <span data-ttu-id="b4e4f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4e4f-105">Property</span></span>     | <span data-ttu-id="b4e4f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b4e4f-106">Type</span></span>   |<span data-ttu-id="b4e4f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b4e4f-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4e4f-108">Кустомдомаинцертификате</span><span class="sxs-lookup"><span data-stu-id="b4e4f-108">customDomainCertificate</span></span>|<span data-ttu-id="b4e4f-109">String</span><span class="sxs-lookup"><span data-stu-id="b4e4f-109">String</span></span>|<span data-ttu-id="b4e4f-110">Сведения о сертификате, связанном с приложением при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="b4e4f-111">NULL при использовании домена по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="b4e4f-112">Екстерналаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="b4e4f-112">externalAuthenticationType</span></span>|<span data-ttu-id="b4e4f-113">String</span><span class="sxs-lookup"><span data-stu-id="b4e4f-113">String</span></span>|<span data-ttu-id="b4e4f-114">Detailed: параметры предварительной проверки подлинности для возможных значений `passthru`приложения `aadPreAuthentication`:,.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="b4e4f-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="b4e4f-115">externalUrl</span></span>|<span data-ttu-id="b4e4f-116">String</span><span class="sxs-lookup"><span data-stu-id="b4e4f-116">String</span></span>|<span data-ttu-id="b4e4f-117">Опубликованный внешний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-117">The published external url for the application.</span></span> <span data-ttu-id="b4e4f-118">Напримерhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="b4e4f-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="b4e4f-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="b4e4f-119">internalUrl</span></span>|<span data-ttu-id="b4e4f-120">String</span><span class="sxs-lookup"><span data-stu-id="b4e4f-120">String</span></span>|<span data-ttu-id="b4e4f-121">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-121">The internal url of the application.</span></span> <span data-ttu-id="b4e4f-122">Напримерhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="b4e4f-122">For example https://intranet/</span></span> |
|<span data-ttu-id="b4e4f-123">Исонпремпублишинженаблед</span><span class="sxs-lookup"><span data-stu-id="b4e4f-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="b4e4f-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e4f-124">Boolean</span></span>|<span data-ttu-id="b4e4f-125">Указывает, выполняется ли публикация приложения в данный момент.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="b4e4f-126">Аппликатионсервертимеаут</span><span class="sxs-lookup"><span data-stu-id="b4e4f-126">applicationServerTimeout</span></span>|<span data-ttu-id="b4e4f-127">String</span><span class="sxs-lookup"><span data-stu-id="b4e4f-127">String</span></span>|<span data-ttu-id="b4e4f-128">Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="b4e4f-129">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="b4e4f-130">Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="b4e4f-131">Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".</span><span class="sxs-lookup"><span data-stu-id="b4e4f-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="b4e4f-132">Истранслатехоссеадеренаблед</span><span class="sxs-lookup"><span data-stu-id="b4e4f-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="b4e4f-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e4f-133">Boolean</span></span>|<span data-ttu-id="b4e4f-134">Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="b4e4f-135">Сюда входит настройка правильного сайта для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4e4f-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4e4f-136">JSON representation</span></span>

<span data-ttu-id="b4e4f-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4e4f-137">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
