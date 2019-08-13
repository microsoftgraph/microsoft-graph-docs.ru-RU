---
title: тип перечисления Емаилцертификатетипе
description: Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c6c4a6943fada88dc9a30c9e81d45705153dfde1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357189"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="98301-103">тип перечисления Емаилцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="98301-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="98301-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98301-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98301-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98301-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98301-106">Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.</span><span class="sxs-lookup"><span data-stu-id="98301-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="98301-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="98301-107">Members</span></span>
|<span data-ttu-id="98301-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="98301-108">Member</span></span>|<span data-ttu-id="98301-109">Значение</span><span class="sxs-lookup"><span data-stu-id="98301-109">Value</span></span>|<span data-ttu-id="98301-110">Описание</span><span class="sxs-lookup"><span data-stu-id="98301-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98301-111">none</span><span class="sxs-lookup"><span data-stu-id="98301-111">none</span></span>|<span data-ttu-id="98301-112">нуль</span><span class="sxs-lookup"><span data-stu-id="98301-112">0</span></span>|<span data-ttu-id="98301-113">Не используйте сертификат в качестве источника.</span><span class="sxs-lookup"><span data-stu-id="98301-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="98301-114">certificate</span><span class="sxs-lookup"><span data-stu-id="98301-114">certificate</span></span>|<span data-ttu-id="98301-115">1,1</span><span class="sxs-lookup"><span data-stu-id="98301-115">1</span></span>|<span data-ttu-id="98301-116">Используйте сертификат для источника сертификата.</span><span class="sxs-lookup"><span data-stu-id="98301-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="98301-117">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="98301-117">derivedCredential</span></span>|<span data-ttu-id="98301-118">2</span><span class="sxs-lookup"><span data-stu-id="98301-118">2</span></span>|<span data-ttu-id="98301-119">Использование производных учетных данных для источника сертификатов.</span><span class="sxs-lookup"><span data-stu-id="98301-119">Use a derived credential for certificate source.</span></span>|



