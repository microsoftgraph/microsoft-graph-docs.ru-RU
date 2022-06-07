---
title: Тип ресурса loginPageTextVisibilitySettings
description: Содержит сведения о фирменной символике организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a74e2ea48d8aa39f6e12a6c5c5908d72d445898e
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924115"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>Тип ресурса loginPageTextVisibilitySettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это сложный тип, представляющий различные тексты, которые могут быть скрыты на странице входа клиента.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| hideAccountResetCredentials | Boolean | Возможность скрыть гиперссылки самостоятельного сброса пароля (SSPR), такие как "Не удается получить доступ к учетной записи?", "Забыли пароль" и "Сбросить его сейчас" в форме входа. |
| hideCannotAccessYourAccount | Boolean | Возможность скрыть самостоятельный сброс пароля (SSPR) "Не удается получить доступ к учетной записи?" гиперссылка на форму входа. |
| hideForgotMyPassword | Boolean | Возможность скрыть гиперссылку самостоятельного сброса пароля (SSPR) "Забыли пароль" в форме входа. |
| hideResetItNow | Boolean | Возможность скрыть гиперссылку самостоятельного сброса пароля (SSPR) "сбросить сейчас" на форме входа. |
| hideTermsOfUse | Boolean | Возможность скрыть гиперссылку "Условия использования" в нижнем колонтитуле. |
| hidePrivacyAndCookies | Boolean | Возможность скрыть гиперссылку "Конфиденциальность & cookies" в нижнем колонтитуле. |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loginPageTextVisibilitySettings",
  "hideAccountResetCredentials": "Boolean",
  "hideCannotAccessYourAccount": "Boolean",
  "hideForgotMyPassword": "Boolean",
  "hidePrivacyAndCookies": "Boolean",
  "hideResetItNow": "Boolean",
  "hideTermsOfUse": "Boolean"
}
```
