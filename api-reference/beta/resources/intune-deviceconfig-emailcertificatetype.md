---
title: тип перечисления Емаилцертификатетипе
description: Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 691923c70c89d2f29cb45f6f3a994bbc919a7d56
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705976"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="e955d-103">тип перечисления Емаилцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="e955d-103">emailCertificateType enum type</span></span>

<span data-ttu-id="e955d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e955d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e955d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e955d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e955d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e955d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e955d-107">Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e955d-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="e955d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e955d-108">Members</span></span>
|<span data-ttu-id="e955d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e955d-109">Member</span></span>|<span data-ttu-id="e955d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e955d-110">Value</span></span>|<span data-ttu-id="e955d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e955d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e955d-112">none</span><span class="sxs-lookup"><span data-stu-id="e955d-112">none</span></span>|<span data-ttu-id="e955d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e955d-113">0</span></span>|<span data-ttu-id="e955d-114">Не используйте сертификат в качестве источника.</span><span class="sxs-lookup"><span data-stu-id="e955d-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="e955d-115">certificate</span><span class="sxs-lookup"><span data-stu-id="e955d-115">certificate</span></span>|<span data-ttu-id="e955d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e955d-116">1</span></span>|<span data-ttu-id="e955d-117">Используйте сертификат для источника сертификата.</span><span class="sxs-lookup"><span data-stu-id="e955d-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="e955d-118">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="e955d-118">derivedCredential</span></span>|<span data-ttu-id="e955d-119">2</span><span class="sxs-lookup"><span data-stu-id="e955d-119">2</span></span>|<span data-ttu-id="e955d-120">Использование производных учетных данных для источника сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e955d-120">Use a derived credential for certificate source.</span></span>|





