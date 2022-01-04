---
title: тип enum macOSSoftwareUpdateBehavior
description: Обновление параметров поведения для обновлений программного обеспечения macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a0fa894d17e126287ccb1e1c63e36160cf2dcd3e
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712084"
---
# <a name="macossoftwareupdatebehavior-enum-type"></a>тип enum macOSSoftwareUpdateBehavior

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление параметров поведения для обновлений программного обеспечения macOS.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Не настроено.|
|default|1|Скачайте и/или установите обновление программного обеспечения в зависимости от текущего состояния устройства.|
|downloadOnly|2|Скачайте обновление программного обеспечения без его установки.|
|installASAP|3|Установка уже загруженного обновления программного обеспечения.|
|notifyOnly|4|Скачайте обновление программного обеспечения и уведомите пользователя через App Store.|
|installLater|5|Скачайте обновление программного обеспечения и установите его позже.|




