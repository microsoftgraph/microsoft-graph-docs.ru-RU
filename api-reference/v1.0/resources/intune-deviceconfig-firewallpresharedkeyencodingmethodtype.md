---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ad59a11aec2fbf715657de95eb3aafc778da43a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947829"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="d2963-103">Тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="d2963-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="d2963-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2963-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2963-105">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d2963-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="d2963-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d2963-106">Members</span></span>
|<span data-ttu-id="d2963-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d2963-107">Member</span></span>|<span data-ttu-id="d2963-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d2963-108">Value</span></span>|<span data-ttu-id="d2963-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d2963-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2963-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d2963-110">deviceDefault</span></span>|<span data-ttu-id="d2963-111">0</span><span class="sxs-lookup"><span data-stu-id="d2963-111">0</span></span>|<span data-ttu-id="d2963-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d2963-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d2963-113">Нет</span><span class="sxs-lookup"><span data-stu-id="d2963-113">none</span></span>|<span data-ttu-id="d2963-114">1</span><span class="sxs-lookup"><span data-stu-id="d2963-114">1</span></span>|<span data-ttu-id="d2963-115">Предварительный ключ не кодируются.</span><span class="sxs-lookup"><span data-stu-id="d2963-115">Preshared key is not encoded.</span></span> <span data-ttu-id="d2963-116">Вместо этого он будет храниться в формате Юникода</span><span class="sxs-lookup"><span data-stu-id="d2963-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="d2963-117">utF8</span><span class="sxs-lookup"><span data-stu-id="d2963-117">utF8</span></span>|<span data-ttu-id="d2963-118">2</span><span class="sxs-lookup"><span data-stu-id="d2963-118">2</span></span>|<span data-ttu-id="d2963-119">Кодирование предварительный ключ, используя UTF-8</span><span class="sxs-lookup"><span data-stu-id="d2963-119">Encode the preshared key using UTF-8</span></span>|



