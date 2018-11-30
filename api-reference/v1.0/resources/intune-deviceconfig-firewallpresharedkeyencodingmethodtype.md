---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
ms.openlocfilehash: 238d2b0845b0d79ea109cea5b326914815d600de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026604"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="bcc0e-103">Тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="bcc0e-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="bcc0e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bcc0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcc0e-105">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="bcc0e-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="bcc0e-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="bcc0e-106">Members</span></span>
|<span data-ttu-id="bcc0e-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="bcc0e-107">Member</span></span>|<span data-ttu-id="bcc0e-108">Значение</span><span class="sxs-lookup"><span data-stu-id="bcc0e-108">Value</span></span>|<span data-ttu-id="bcc0e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc0e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc0e-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="bcc0e-110">deviceDefault</span></span>|<span data-ttu-id="bcc0e-111">0</span><span class="sxs-lookup"><span data-stu-id="bcc0e-111">0</span></span>|<span data-ttu-id="bcc0e-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="bcc0e-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="bcc0e-113">Нет</span><span class="sxs-lookup"><span data-stu-id="bcc0e-113">none</span></span>|<span data-ttu-id="bcc0e-114">1</span><span class="sxs-lookup"><span data-stu-id="bcc0e-114">1</span></span>|<span data-ttu-id="bcc0e-115">Предварительный ключ не кодируются.</span><span class="sxs-lookup"><span data-stu-id="bcc0e-115">Preshared key is not encoded.</span></span> <span data-ttu-id="bcc0e-116">Вместо этого он будет храниться в формате Юникода</span><span class="sxs-lookup"><span data-stu-id="bcc0e-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="bcc0e-117">utF8</span><span class="sxs-lookup"><span data-stu-id="bcc0e-117">utF8</span></span>|<span data-ttu-id="bcc0e-118">2</span><span class="sxs-lookup"><span data-stu-id="bcc0e-118">2</span></span>|<span data-ttu-id="bcc0e-119">Кодирование предварительный ключ, используя UTF-8</span><span class="sxs-lookup"><span data-stu-id="bcc0e-119">Encode the preshared key using UTF-8</span></span>|



