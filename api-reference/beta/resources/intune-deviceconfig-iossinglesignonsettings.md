---
title: Тип ресурса iosSingleSignOnSettings
description: операций ввода-вывода параметров проверки подлинности Kerberos для единого входа
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421321"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="38acf-103">Тип ресурса iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="38acf-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="38acf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38acf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38acf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38acf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38acf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38acf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38acf-107">операций ввода-вывода параметров проверки подлинности Kerberos для единого входа</span><span class="sxs-lookup"><span data-stu-id="38acf-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="38acf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="38acf-108">Properties</span></span>
|<span data-ttu-id="38acf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="38acf-109">Property</span></span>|<span data-ttu-id="38acf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="38acf-110">Type</span></span>|<span data-ttu-id="38acf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38acf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38acf-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="38acf-112">allowedAppsList</span></span>|<span data-ttu-id="38acf-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="38acf-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="38acf-114">Список идентификаторов приложения, которые могут использовать это имя входа.</span><span class="sxs-lookup"><span data-stu-id="38acf-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="38acf-115">Если это поле указан, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="38acf-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="38acf-116">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="38acf-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="38acf-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="38acf-117">allowedUrls</span></span>|<span data-ttu-id="38acf-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="38acf-118">String collection</span></span>|<span data-ttu-id="38acf-119">Список URL-адресов HTTP для соответствия для использования этим именем входа.</span><span class="sxs-lookup"><span data-stu-id="38acf-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="38acf-120">С помощью операций ввода-вывода 9.0 или более поздней версии могут быть использованы подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="38acf-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="38acf-121">displayName</span><span class="sxs-lookup"><span data-stu-id="38acf-121">displayName</span></span>|<span data-ttu-id="38acf-122">String</span><span class="sxs-lookup"><span data-stu-id="38acf-122">String</span></span>|<span data-ttu-id="38acf-123">Отображаемое имя параметры входа в систему на получающей устройства.</span><span class="sxs-lookup"><span data-stu-id="38acf-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="38acf-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38acf-124">kerberosPrincipalName</span></span>|<span data-ttu-id="38acf-125">String</span><span class="sxs-lookup"><span data-stu-id="38acf-125">String</span></span>|<span data-ttu-id="38acf-126">Имя участника Kerberos.</span><span class="sxs-lookup"><span data-stu-id="38acf-126">A Kerberos principal name.</span></span> <span data-ttu-id="38acf-127">Если этот параметр не указан, пользователю предлагается ввести один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="38acf-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="38acf-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="38acf-128">kerberosRealm</span></span>|<span data-ttu-id="38acf-129">String</span><span class="sxs-lookup"><span data-stu-id="38acf-129">String</span></span>|<span data-ttu-id="38acf-130">Имя сферы Kerberos.</span><span class="sxs-lookup"><span data-stu-id="38acf-130">A Kerberos realm name.</span></span> <span data-ttu-id="38acf-131">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="38acf-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38acf-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="38acf-132">Relationships</span></span>
<span data-ttu-id="38acf-133">Нет</span><span class="sxs-lookup"><span data-stu-id="38acf-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38acf-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38acf-134">JSON Representation</span></span>
<span data-ttu-id="38acf-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38acf-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```




