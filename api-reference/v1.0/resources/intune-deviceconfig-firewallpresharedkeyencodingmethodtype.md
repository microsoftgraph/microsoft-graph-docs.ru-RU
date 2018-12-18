---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
author: tfitzmac
ms.openlocfilehash: b8ab119c58aec6e62c0a32ccf310f43eab029573
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343591"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="36907-103">Тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="36907-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="36907-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36907-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36907-105">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="36907-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="36907-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="36907-106">Members</span></span>
|<span data-ttu-id="36907-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="36907-107">Member</span></span>|<span data-ttu-id="36907-108">Значение</span><span class="sxs-lookup"><span data-stu-id="36907-108">Value</span></span>|<span data-ttu-id="36907-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36907-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36907-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="36907-110">deviceDefault</span></span>|<span data-ttu-id="36907-111">0</span><span class="sxs-lookup"><span data-stu-id="36907-111">0</span></span>|<span data-ttu-id="36907-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="36907-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="36907-113">none</span><span class="sxs-lookup"><span data-stu-id="36907-113">none</span></span>|<span data-ttu-id="36907-114">1</span><span class="sxs-lookup"><span data-stu-id="36907-114">1</span></span>|<span data-ttu-id="36907-115">Предварительный ключ не кодируются.</span><span class="sxs-lookup"><span data-stu-id="36907-115">Preshared key is not encoded.</span></span> <span data-ttu-id="36907-116">Вместо этого он будет храниться в формате Юникода</span><span class="sxs-lookup"><span data-stu-id="36907-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="36907-117">utF8</span><span class="sxs-lookup"><span data-stu-id="36907-117">utF8</span></span>|<span data-ttu-id="36907-118">2</span><span class="sxs-lookup"><span data-stu-id="36907-118">2</span></span>|<span data-ttu-id="36907-119">Кодирование предварительный ключ, используя UTF-8</span><span class="sxs-lookup"><span data-stu-id="36907-119">Encode the preshared key using UTF-8</span></span>|



