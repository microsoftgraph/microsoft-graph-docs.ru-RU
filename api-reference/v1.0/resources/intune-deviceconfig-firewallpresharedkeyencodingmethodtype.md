---
title: брандмауэрPreSharedKeyEncodingMethodType
description: Возможные значения брандмауэраPreSharedKeyEncodingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 200177be7f8258965067f12cace3b163aefc6b78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755058"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="23ef4-103">брандмауэрPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="23ef4-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="23ef4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ef4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23ef4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23ef4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23ef4-106">Возможные значения брандмауэраPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="23ef4-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="23ef4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="23ef4-107">Members</span></span>
|<span data-ttu-id="23ef4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="23ef4-108">Member</span></span>|<span data-ttu-id="23ef4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="23ef4-109">Value</span></span>|<span data-ttu-id="23ef4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23ef4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ef4-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="23ef4-111">deviceDefault</span></span>|<span data-ttu-id="23ef4-112">0</span><span class="sxs-lookup"><span data-stu-id="23ef4-112">0</span></span>|<span data-ttu-id="23ef4-113">Нет значения, настроенного Intune, не переопределять настроенное пользователем значение по умолчанию устройства</span><span class="sxs-lookup"><span data-stu-id="23ef4-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="23ef4-114">нет</span><span class="sxs-lookup"><span data-stu-id="23ef4-114">none</span></span>|<span data-ttu-id="23ef4-115">1</span><span class="sxs-lookup"><span data-stu-id="23ef4-115">1</span></span>|<span data-ttu-id="23ef4-116">Предустанавливаемая клавиша не закодирована.</span><span class="sxs-lookup"><span data-stu-id="23ef4-116">Preshared key is not encoded.</span></span> <span data-ttu-id="23ef4-117">Вместо этого он хранится в широкоформатном формате</span><span class="sxs-lookup"><span data-stu-id="23ef4-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="23ef4-118">utF8</span><span class="sxs-lookup"><span data-stu-id="23ef4-118">utF8</span></span>|<span data-ttu-id="23ef4-119">2</span><span class="sxs-lookup"><span data-stu-id="23ef4-119">2</span></span>|<span data-ttu-id="23ef4-120">Кодирование предшарного ключа с помощью UTF-8</span><span class="sxs-lookup"><span data-stu-id="23ef4-120">Encode the preshared key using UTF-8</span></span>|




