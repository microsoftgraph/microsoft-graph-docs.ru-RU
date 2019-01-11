---
title: Тип ресурса educationSynchronizationConnectionSettings
description: 'Представляет параметры подключения поставщика. Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 17fedb5094016bd3df3bd8262390eaa7eeb37537
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841771"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="8ca22-104">Тип ресурса educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="8ca22-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="8ca22-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ca22-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ca22-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ca22-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ca22-107">Представляет параметры подключения поставщика.</span><span class="sxs-lookup"><span data-stu-id="8ca22-107">Represents the provider connection settings.</span></span> <span data-ttu-id="8ca22-108">Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="8ca22-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="8ca22-109">**Примечание:** В данном сложном типе абстрактный.</span><span class="sxs-lookup"><span data-stu-id="8ca22-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="8ca22-110">Обращайтесь к определенным типам параметров подключения из списка.</span><span class="sxs-lookup"><span data-stu-id="8ca22-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="8ca22-111">Производные типы</span><span class="sxs-lookup"><span data-stu-id="8ca22-111">Derived types</span></span>
| <span data-ttu-id="8ca22-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8ca22-112">Type</span></span> | <span data-ttu-id="8ca22-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8ca22-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="8ca22-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="8ca22-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="8ca22-115">Этот тип используется для предоставления параметров подключения OAuth1.</span><span class="sxs-lookup"><span data-stu-id="8ca22-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="8ca22-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="8ca22-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="8ca22-117">Этот тип используется для предоставления параметров подключения OAuth2 предоставить учетные данные клиента.</span><span class="sxs-lookup"><span data-stu-id="8ca22-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ca22-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ca22-118">Properties</span></span>

| <span data-ttu-id="8ca22-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ca22-119">Property</span></span> | <span data-ttu-id="8ca22-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8ca22-120">Type</span></span> | <span data-ttu-id="8ca22-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8ca22-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8ca22-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="8ca22-122">**clientId**</span></span> | <span data-ttu-id="8ca22-123">Строка</span><span class="sxs-lookup"><span data-stu-id="8ca22-123">String</span></span> |  <span data-ttu-id="8ca22-124">Идентификатор клиента, используемого для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="8ca22-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="8ca22-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="8ca22-125">**clientSecret**</span></span> | <span data-ttu-id="8ca22-126">Строка</span><span class="sxs-lookup"><span data-stu-id="8ca22-126">String</span></span> |  <span data-ttu-id="8ca22-127">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="8ca22-127">Client secret to authenticate the connection to the provider.</span></span> |
