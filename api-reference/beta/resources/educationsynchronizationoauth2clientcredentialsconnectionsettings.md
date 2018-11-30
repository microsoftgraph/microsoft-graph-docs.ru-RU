---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings ресурсов
description: При OAuth2 предоставить учетные данные клиента будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.
ms.openlocfilehash: 901fabb802d4ed5fa0c99538e52b9a07199eb298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080541"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="3453c-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings ресурсов</span><span class="sxs-lookup"><span data-stu-id="3453c-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="3453c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3453c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3453c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3453c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3453c-106">При [OAuth2 предоставить учетные данные клиента](https://tools.ietf.org/html/rfc6749#section-4.4) будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="3453c-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="3453c-107">На основе [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3453c-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3453c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3453c-108">Properties</span></span>

| <span data-ttu-id="3453c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3453c-109">Property</span></span> | <span data-ttu-id="3453c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3453c-110">Type</span></span> | <span data-ttu-id="3453c-111">Description</span><span class="sxs-lookup"><span data-stu-id="3453c-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3453c-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="3453c-112">**tokenUrl**</span></span> | <span data-ttu-id="3453c-113">String</span><span class="sxs-lookup"><span data-stu-id="3453c-113">String</span></span> | <span data-ttu-id="3453c-114">URL-адрес для получения маркера доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="3453c-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="3453c-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="3453c-115">**scope**</span></span> | <span data-ttu-id="3453c-116">String</span><span class="sxs-lookup"><span data-stu-id="3453c-116">String</span></span> | <span data-ttu-id="3453c-117">[Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="3453c-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3453c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3453c-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
