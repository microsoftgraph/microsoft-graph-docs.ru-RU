---
title: тип перечисления Емаилцертификатетипе
description: Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d2f5e4add7f67c6b772aa903d4e3b860b67ecbf5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460103"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="0dd11-103">тип перечисления Емаилцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="0dd11-103">emailCertificateType enum type</span></span>

<span data-ttu-id="0dd11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dd11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dd11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dd11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dd11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0dd11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dd11-107">Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0dd11-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="0dd11-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0dd11-108">Members</span></span>
|<span data-ttu-id="0dd11-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0dd11-109">Member</span></span>|<span data-ttu-id="0dd11-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0dd11-110">Value</span></span>|<span data-ttu-id="0dd11-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0dd11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dd11-112">Нет</span><span class="sxs-lookup"><span data-stu-id="0dd11-112">none</span></span>|<span data-ttu-id="0dd11-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0dd11-113">0</span></span>|<span data-ttu-id="0dd11-114">Не используйте сертификат в качестве источника.</span><span class="sxs-lookup"><span data-stu-id="0dd11-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="0dd11-115">certificate</span><span class="sxs-lookup"><span data-stu-id="0dd11-115">certificate</span></span>|<span data-ttu-id="0dd11-116">1,1</span><span class="sxs-lookup"><span data-stu-id="0dd11-116">1</span></span>|<span data-ttu-id="0dd11-117">Используйте сертификат для источника сертификата.</span><span class="sxs-lookup"><span data-stu-id="0dd11-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="0dd11-118">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="0dd11-118">derivedCredential</span></span>|<span data-ttu-id="0dd11-119">2</span><span class="sxs-lookup"><span data-stu-id="0dd11-119">2</span></span>|<span data-ttu-id="0dd11-120">Использование производных учетных данных для источника сертификатов.</span><span class="sxs-lookup"><span data-stu-id="0dd11-120">Use a derived credential for certificate source.</span></span>|



