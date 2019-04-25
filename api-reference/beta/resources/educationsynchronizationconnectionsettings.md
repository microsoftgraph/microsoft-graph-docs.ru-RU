---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542997"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="2eaae-104">Тип ресурса Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="2eaae-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2eaae-105">Представляет параметры подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="2eaae-105">Represents the provider connection settings.</span></span> <span data-ttu-id="2eaae-106">Это позволяет системе узнать, как подключаться к API поставщика.</span><span class="sxs-lookup"><span data-stu-id="2eaae-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="2eaae-107">**Примечание:** Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="2eaae-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="2eaae-108">Ознакомьтесь со списками определенных типов параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="2eaae-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="2eaae-109">ПроизВодные типы</span><span class="sxs-lookup"><span data-stu-id="2eaae-109">Derived types</span></span>
| <span data-ttu-id="2eaae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2eaae-110">Type</span></span> | <span data-ttu-id="2eaae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2eaae-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="2eaae-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="2eaae-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="2eaae-113">Используйте этот тип для предоставления параметров подключения OAuth1.</span><span class="sxs-lookup"><span data-stu-id="2eaae-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="2eaae-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="2eaae-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="2eaae-115">Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="2eaae-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="2eaae-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="2eaae-116">Properties</span></span>

| <span data-ttu-id="2eaae-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2eaae-117">Property</span></span> | <span data-ttu-id="2eaae-118">Тип</span><span class="sxs-lookup"><span data-stu-id="2eaae-118">Type</span></span> | <span data-ttu-id="2eaae-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2eaae-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2eaae-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="2eaae-120">**clientId**</span></span> | <span data-ttu-id="2eaae-121">String</span><span class="sxs-lookup"><span data-stu-id="2eaae-121">String</span></span> |  <span data-ttu-id="2eaae-122">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="2eaae-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="2eaae-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="2eaae-123">**clientSecret**</span></span> | <span data-ttu-id="2eaae-124">String</span><span class="sxs-lookup"><span data-stu-id="2eaae-124">String</span></span> |  <span data-ttu-id="2eaae-125">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="2eaae-125">Client secret to authenticate the connection to the provider.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
